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
    stage('Build') {
      parallel {
        stage('') {
          steps {
            echo 'Building'
          }
        }
        stage('Build') {
          steps {
            echo 'Demo Build '
          }
        }
        stage('BUILD') {
          steps {
            echo 'Learn Building '
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