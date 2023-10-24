pipeline{
    agent any
    stages{
        stage ('BUILD') {
            steps{
                echo "This is build stage"
                sh 'sleep 5'
            }
        }

        stage ('TEST PARALLEL'){
            parallel {
                stage('TEST ON CHROME') {
                    steps{
                        echo "This is test on Chrome Browser"
                        sh 'ls -lrt'
                    }    
                }
                stage('TEST ON SAFARI') {
                    steps{
                        echo "This is test on SAFARI Browser"
                        sh 'sleep 3'
                    }    
                }
            } 
        } 


        stage ('Deploy') {
            agent { label 'Shre-slave1' }
            steps{
                echo "this is deploy stage"
                sh 'df -h'
            }
        }

    }
}