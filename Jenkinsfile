pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        parallel(
          "Compile": {
            echo 'compile'
            
          },
          "bla": {
            withMaven()
            sh 'echo "hallo"'
            
          }
        )
      }
    }
    stage('Test') {
      steps {
        echo 'hallo'
      }
    }
    stage('Publish Snapshot') {
      steps {
        echo 'hallo'
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
      }
    }
  }
}