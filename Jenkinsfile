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
                              sh 'gcc helloworld.c -o helloworld'
                          }
                 }
                 stage('Testing App') {
                          steps {
                                echo "Running final tests"
                                sh 'ls -liah'
                                sh 'cat helloworld.c'
                                sh './helloworld'
                           }  
                  }
         }
}
