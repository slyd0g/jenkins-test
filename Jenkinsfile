pipeline {
         agent any

         parameters {
                 string(name: 'BRANCH', defaultValue: 'main', description: 'Branch to build')
         }
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
