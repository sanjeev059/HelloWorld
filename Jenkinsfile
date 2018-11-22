pipeline {
  agent any
  stages {
    stage('Build Prod') {
      parallel {
        stage('Build Prod') {
          steps {
            echo 'In Production'
          }
        }
        stage('Build Learn') {
          steps {
            echo 'In Learn'
          }
        }
      }
    }
    stage('Promote Prod') {
      parallel {
        stage('Promote Prod') {
          steps {
            echo 'Build Prod'
          }
        }
        stage('Promote Learn') {
          steps {
            echo 'In Learn Promote'
          }
        }
      }
    }
    stage('Deploy Prod') {
      parallel {
        stage('Deploy Prod') {
          steps {
            echo 'Deployed'
          }
        }
        stage('Deploy Learn') {
          steps {
            echo 'In Learn Deploy'
          }
        }
      }
    }
    stage('Test Prod') {
      parallel {
        stage('Test Prod') {
          steps {
            echo 'tested'
          }
        }
        stage('Test Learn') {
          steps {
            echo 'In Learn testing'
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