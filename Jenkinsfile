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
    stage('') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build Prod'
          }
        }
        stage('Build') {
          steps {
            echo 'Demo Build '
          }
        }
        stage('Build') {
          steps {
            echo 'Leran building'
          }
        }
      }
    }
    stage('Deploy ') {
      parallel {
        stage('Deploy ') {
          steps {
            echo 'Deployed'
          }
        }
        stage('DEPLOY') {
          steps {
            echo 'Deploy'
          }
        }
        stage('Deploy') {
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