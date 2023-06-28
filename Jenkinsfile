pipeline {
    agent any

    stages {
        stage('Build') {
          parallel {
              steps {
              echo 'Building..'
            }
          }
        }
        stage('Deploy') {
          parallel {
              steps {
              echo 'Deploy..'
            }
          }
        }
    }
}
