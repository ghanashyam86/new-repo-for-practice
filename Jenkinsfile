pipeline{
    agent {
         node {
              label 'built-in'
              customWorkspace '/mnt/git-repo'
              }
            }
        stages {
            stage ('clone-repo') {
                steps {
                       sh "rm -rf hello-world*"
                      sh "git clone https://github.com/ghanashyam86/hello-world.git"
                      }
                   }
            stage ('build-hello-world-repo') {
                steps {
                    dir ('/mnt/git-repo/hello-world'){
                    sh "mvn clean install"
                  }
                }     
            }
       }
}
