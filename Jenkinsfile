pipeline {
  agent any
  stages {
    stage('Build Learn') {
      steps {
        echo 'In Production'
      }
    }
    stage('Promote Learn') {
      steps {
        echo 'Build Prod'
      }
    }
    stage('Deploy Learn') {
      steps {
        echo 'Deployed'
      }
    }
    stage('Test Learn') {
      parallel {
        stage('Test Learn') {
          steps {
            echo 'tested'
          }
        }
        stage('test1') {
          steps {
            echo 'Test 1'
          }
        }
        stage('Test2') {
          steps {
            echo 'test2'
          }
        }
        stage('Test 3') {
          steps {
            echo 'test3'
          }
        }
        stage('Test4') {
          steps {
            echo 'test4'
          }
        }
        stage('TestN') {
          steps {
            echo 'test N'
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