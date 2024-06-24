pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build..'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing Firebox'
          }
        }

        stage('Testing Chrome') {
          steps {
            echo 'Testing Chrome..'
          }
        }

        stage('Testing Edg') {
          steps {
            echo 'Testing Edg'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}