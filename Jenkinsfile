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
      environment {
        DOCKERHUB_USER = 'Vudujones'
        DOCKERHUB_PASSWORD = 'LargoVista192193.'
      }
      steps {
        sh 'docker login -u $DOCKERHUB_USER -p $DOCKERHUB_PASSWORD'
      }
    }

  }
}