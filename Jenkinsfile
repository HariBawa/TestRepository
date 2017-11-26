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
        stage('Dev Test 2') {
          steps {
            echo 'Additional test 2'
          }
        }
        stage('Dev Test 3') {
          steps {
            echo 'Additional Test 3'
          }
        }
      }
    }
    stage('Dev Deploy ') {
      steps {
        echo 'Deliver to Dev Environment'
        echo 'Deploy Step 2'
        echo 'Deploy Step 3'
      }
    }
  }
  environment {
    author = 'Hari Bawa'
    project = 'Test Project'
  }
}