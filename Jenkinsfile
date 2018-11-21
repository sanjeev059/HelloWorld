pipeline {
  agent any
  stages {
    stage('Production') {
      steps {
        echo 'In Production'
      }
    }
    stage('Build') {
      steps {
        echo 'Building'
      }
    }
    stage('Deploy ') {
      steps {
        echo 'Deployed'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'tested'
          }
        }
        stage('Run test Parellel') {
          steps {
            echo 'hello'
            junit(allowEmptyResults: true, testResults: 'done')
          }
        }
      }
    }
    stage('Artifacts') {
      steps {
        echo 'stored artifacts'
      }
    }
  }
}