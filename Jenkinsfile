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
                      sh "git clone https://github.com/ghanashyam86/hello-world.git"
                      }
                   }
            }
}
