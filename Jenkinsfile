pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'i want to build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I want to test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deployed'
          }
        }

      }
    }

  }
}