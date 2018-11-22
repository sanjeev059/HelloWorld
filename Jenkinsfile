pipeline {
  agent any
  stages {
    stage('Prod') {
      parallel {
        stage('error') {
          steps {
            echo 'In Production'
          }
        }
        stage('') {
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
    stage('build prod') {
      parallel {
        stage('error') {
          steps {
            echo 'Build Prod'
          }
        }
        stage('') {
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
    stage('deploy prod') {
      parallel {
        stage('error') {
          steps {
            echo 'Deployed'
          }
        }
        stage('') {
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
    stage('test prod') {
      parallel {
        stage('error') {
          steps {
            echo 'tested'
          }
        }
        stage('') {
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