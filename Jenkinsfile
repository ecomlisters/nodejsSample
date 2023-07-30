pipeline{
    agent any
    parameters {
        string(defaultValue: "develop", description: 'enter the branch name to use', name: 'branchName')
    }
    stages{
        stage('Checkout'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: "*/${branchName}"]], gitTool: 'jgit', userRemoteConfigs: [[url: "https://github.com/ecomlisters/nodejsSample"]]])
                
            }
        }
    }
}
