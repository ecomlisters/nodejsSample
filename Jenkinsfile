pipeline{
    agent any

    stages {
        stage('Build') {
            steps {
                echo BRANCH_NAME
                git url: 'https://github.com/ecomlisters/nodejsSample'
            }
        }
        stage('Install') {
            steps {
                npm 'install'
            }
        }
        stage('Sonar'){
          when {
            expression {
              BRANCH_NAME == 'main'
              }
          }
         steps{
           script{
              echo 'running Sonar stage ...'
           }
         }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
