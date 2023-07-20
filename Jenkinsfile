pipeline {
         agent any
         stages {
                 stage('Pre-build') {
                 steps {
                     echo 'Starting pre-build!'
                 }
                 }
                 stage('Lint') {
                 steps {
                    echo 'Starting lint!'
                 }
                 }
                 stage('Build') {
                 steps {
                     echo 'Building now!'
                     sh 'ls -liah'
                 }
                 }
                 stage('Push') {
                     steps {
                                echo "App is being pushed to artifact storage"
                                sh 'ls -liah'
                              }
                 
              }
}
}
