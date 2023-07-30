pipeline{
    agent any

    parameters {
      gitParameter branch: '', branchFilter: '.*', defaultValue: '', name: 'branchName', quickFilterEnabled: false, selectedValue: 'NONE', sortMode: 'NONE', tagFilter: '*', type: 'GitParameterDefinition'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building from branch ${branchName}'
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
