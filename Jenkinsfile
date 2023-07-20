pipeline {
         agent any
         stages {
                 stage('Pre-build') {
                 steps {
                     echo 'Starting pre-build!'
                     sh 'cat helloworld.c'
                 }
                 }
                 stage('Lint') {
                 steps {
                    echo 'Starting lint!'
                    sh 'cat helloworld.c'
                 }
                 }
                 stage('Build') {
                 steps {
                     echo 'Building now!'
                     sh 'ls -liah'
                     sh 'cat helloworld.c'
                 }
                 }
                 stage('Push') {
                     steps {
                                echo "App is being pushed to artifact storage"
                                sh 'ls -liah'
                                sh 'cat helloworld.c'
                              }
                 
              }
}
}
