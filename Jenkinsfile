pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'running build'
        git branch: '${branchName}', changelog: false, poll: false, url: 'https://github.com/ecomlisters/nodejsSample'
      }
    }

   
  }
}
