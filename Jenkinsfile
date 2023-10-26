pipeline {
    agent any
    stages{

        stage('BUILD'){
            steps {
                echo "This is Build stage"
                sh '''
                       sleep 5
                       ls -lrt
                   '''   
            }
        }
        stage('TEST') {
            steps {
                echo "This is Test stage"
                sh '''
                        df -h
                   '''

            }
        }

        stage ('DEPLOY') {
            steps {
                echo "This is Deploy stage"
                sh '''
                       sleep 5
                   '''    
            }
        }
    }
}