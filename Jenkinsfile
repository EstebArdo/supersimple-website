pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/EstebArdo/supersimple-website', branch: 'Dev')
      }
    }

    stage('') {
      steps {
        sh 'ls -al'
      }
    }

  }
}