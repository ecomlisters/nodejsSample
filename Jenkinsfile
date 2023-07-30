pipeline{
    agent any

   environment {
     BRANCH_NAME = "${GIT_BRANCH.split("/")[1]}"
  }

    stages {
        stage('Build') {
            steps {
                echo 'Building from branch ${BRANCH_NAME}'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
