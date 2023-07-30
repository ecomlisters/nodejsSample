pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'running build'
        git(url: 'https://github.com/ecomlisters/nodejsSample/', branch: 'main')
      }
    }

    stage('inst') {
      steps {
        npm 'install'
      }
    }

    

  }
}
