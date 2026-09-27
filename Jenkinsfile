pipeline {
    agent any

    stages {

        stage('STAGE7') {
            steps {
                sh 'ls -lrt'
            }
        }

        stage('STAGE2') {
            steps {
                sh '''
                    pwd
                    sleep
                    ls -lrt
                   '''
            }
        }
         
        stage('STAGE3') {
            steps {
                echo "THIS IS stage 3 "
            }
        }
        stage('STAGE4') {
            steps {
               sh ' echo this is stage4'
            }
        }
    }
}