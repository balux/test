pipeline {
  agent any
  stages {
    stage('Compile') {
      parallel {
        stage('Compile') {
          steps {
            echo 'compile'
            library 'nextlayerci'
          }
        }
        stage('npm') {
          steps {
            sh '''npm install
'''
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'hallo'
      }
    }
    stage('Publish Snapshot') {
      parallel {
        stage('Publish Snapshot') {
          steps {
            echo 'hallo'
          }
        }
        stage('Test') {
          steps {
            echo 'hallo'
          }
        }
      }
    }
    stage('QA') {
      steps {
        echo 'hallo'
        input 'Promote Build?'
      }
    }
    stage('Deploy Production') {
      steps {
        echo 'hallo'
        waitUntil() {
          sh 'echo hallo'
        }
        
      }
    }
  }
}