pipeline {
  agent none
  stages {
    stage('build') {
      steps {
        git(url: 'https://github.com/ecomlisters/nodejsSample/', branch: 'main')
      }
    }

    stage('install') {
      steps {
        npm 'npm install'
      }
    }

  }
}