pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building...'
      }
    }

    stage('test') {
      parallel {
        stage('test firefox') {
          steps {
            sh 'echo "test firefox"'
          }
        }

        stage('test chrome') {
          steps {
            sh 'echo "test chrome"'
          }
        }

        stage('test edge') {
          steps {
            sh 'echo "test edge"'
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