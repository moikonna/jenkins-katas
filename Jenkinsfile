pipeline {
  agent any
  stages {
    stage('yeet') {
      parallel {
        stage('yeet') {
          steps {
            sh 'echo "hello world"'
          }
        }

        stage('build') {
          agent {
            docker {
              image 'gradle:6-jdk11'
            }

          }
          steps {
            sh 'ci/build-app.sh'
          }
        }

      }
    }

  }
}