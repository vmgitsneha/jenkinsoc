pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building'
      }
    }

    stage('dev') {
      parallel {
        stage('dev') {
          steps {
            echo 'dev'
          }
        }

        stage('qa') {
          steps {
            echo 'qa'
          }
        }

      }
    }

    stage('prod') {
      steps {
        echo 'od'
      }
    }

  }
}