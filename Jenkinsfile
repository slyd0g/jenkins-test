pipeline {
         agent any

         parameters {
                 string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                 text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
                 booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
                 choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
                 password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
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
