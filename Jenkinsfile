pipeline {
  agent any
  stages {
    stage('Production') {
      parallel {
        stage('Production') {
          steps {
            echo 'In Production'
          }
        }
        stage('Demo') {
          steps {
            echo 'Am Demo'
          }
        }
        stage('Learn') {
          steps {
            echo 'Learn'
          }
        }
      }
    }
    stage('error') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build Prod'
          }
        }
        stage('Build Demo') {
          steps {
            echo 'Demo Build '
          }
        }
        stage('Build Learn') {
          steps {
            echo 'Leran building'
          }
        }
      }
    }
    stage('Deploy ') {
      parallel {
        stage('Deploy Prod') {
          steps {
            echo 'Deployed'
          }
        }
        stage('Deploy demo') {
          steps {
            echo 'Deploy'
          }
        }
        stage('Deploy Learn') {
          steps {
            echo 'Learn Deploy'
          }
        }
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
        stage('TEST') {
          steps {
            echo 'AM testing '
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