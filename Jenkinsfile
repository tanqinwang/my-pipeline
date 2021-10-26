pipeline {
  agent {
    docker {
      image 'golang'
    }

  }
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'go version'
          }
        }

        stage('test') {
          steps {
            timestamps() {
              echo 'test'
            }

          }
        }

      }
    }

  }
}