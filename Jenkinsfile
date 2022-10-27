pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed'
      }
    }

    stage('Test statges') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Running Test1'
          }
        }

        stage('Test2') {
          steps {
            echo 'Running Test2'
          }
        }

      }
    }

    stage('Deploy') {
      parallel {
        stage('DeployFirst') {
          steps {
            echo 'Deploy First Step Completed'
          }
        }

        stage('DeployFinal') {
          steps {
            echo 'Depoly Final Completed'
          }
        }

      }
    }

  }
}