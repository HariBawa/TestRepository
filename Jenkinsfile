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
      parallel {
        stage('Dev Test') {
          steps {
            echo 'Automated Test on Dev Environment'
          }
        }
        stage('Dev Test Step 2') {
          steps {
            echo 'Step 2 Testing'
          }
        }
        stage('Dev Test Step 3') {
          steps {
            echo 'Dev 3 Step Testing'
          }
        }
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