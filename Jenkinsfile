pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/EstebArdo/supersimple-website', branch: 'Dev')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -al'
      }
    }

    stage('DockerHub Login') {
      steps {
        sh 'docker login -u $DOCKERHUB_USER -p $DOCKERHUB_PASSWORD'
      }
    }

  }
}