pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'i want to plan my application development'
      }
    }

    stage('code') {
      steps {
        echo 'development team perform the app development'
      }
    }

    stage('build') {
      steps {
        echo 'build the application'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing team perform the test activitys'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy the war files'
          }
        }

        stage('Release') {
          steps {
            echo 'move to release'
          }
        }

        stage('Operate') {
          steps {
            echo 'Test application functionality'
          }
        }

      }
    }

  }
}