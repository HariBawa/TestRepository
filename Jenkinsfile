pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        sh 'echo "This is initialize step"'
      }
    }
    stage('Build') {
      steps {
        echo 'This is Build Stage'
      }
    }
    stage('Dev Test') {
      steps {
        echo 'Automated Test on Dev Environment'
      }
    }
    stage('Dev Deploy ') {
      steps {
        echo 'Deliver to Dev Environment'
      }
    }
  }
  environment {
    author = 'Hari Bawa'
    project = 'Test Project'
  }
}