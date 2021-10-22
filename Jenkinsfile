pipeline {
  agent {
    label 'mac'
  }
  stages {
    stage('Build') {
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

    stage('Deploy') {
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