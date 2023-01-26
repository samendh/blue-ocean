pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'This is where code is developed'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'This is where code is tested'
          }
        }

        stage('Deploy') {
          steps {
            echo 'This is where code is deployed'
          }
        }

      }
    }

  }
}