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
  }
}