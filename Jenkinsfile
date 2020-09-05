pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('firefox') {
      parallel {
        stage('firefox') {
          steps {
            echo 'testing firefox'
          }
        }

        stage('edge') {
          steps {
            echo 'testing edge'
          }
        }

        stage('chrome') {
          steps {
            echo 'testing chrome'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploying'
      }
    }

  }
}