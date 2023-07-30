pipeline{
    agent any

   environment {
     BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
  }

    stages {
        stage('Build') {
            steps {
                echo BRANCH_NAME
                git branch: BRANCH_NAME, url: 'https://github.com/ecomlisters/nodejsSample'
            }
        }
        stage('Install') {
            steps {
                npm 'install'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
