pipeline {
  agent any
  stages {
    stage('Source Code Checkout') {
      steps {
        sh 'echo "Checkout source code"'
      }
    }

    stage('Build SIT') {
      parallel {
        stage('Build SIT') {
          steps {
            sh 'echo "Build SIT"'
          }
        }

        stage('Build PROD') {
          steps {
            sh 'echo "Build PROD"'
          }
        }

      }
    }

    stage('Deploy SIT to App Center') {
      parallel {
        stage('Deploy SIT to App Center') {
          steps {
            sh 'echo "Deploy SIT to App Center"'
          }
        }

        stage('Deploy PROD to App Center') {
          steps {
            sh 'echo "Deploy SIT to App Center"'
          }
        }

      }
    }

  }
}