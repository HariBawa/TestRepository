pipeline {
  agent {
    docker {
      image 'maven3.3.9-jdk8'
    }
    
  }
  stages {
    stage('Initialize') {
      steps {
        echo 'This is minimal pipeline'
      }
    }
    stage('Build') {
      steps {
        echo 'This is Build Stage'
      }
    }
    stage('Dev Delivery') {
      steps {
        echo 'This is delivery to Dev Environment'
      }
    }
    stage('Dev Test ') {
      steps {
        echo 'This is test stage'
      }
    }
  }
}