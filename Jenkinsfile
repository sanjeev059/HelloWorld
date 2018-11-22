pipeline {
  agent any
  stages {
    stage('Build Prod') {
      steps {
        echo 'In Production'
      }
    }
    stage('Promote Prod') {
      steps {
        echo 'Build Prod'
      }
    }
    stage('Deploy Prod') {
      steps {
        echo 'Deployed'
      }
    }
    stage('Test Prod') {
      steps {
        echo 'tested'
      }
    }
    stage('Artifacts') {
      steps {
        echo 'stored artifacts'
      }
    }
  }
}