pipeline{
    agent any
    stages{
        stage ('BUILD') {
            steps{
                echo "This is build stage"
                sh 'sleep 5'
            }
        }

        stage ('TEST'){
            steps{
                echo "This is Test stage"
                sh 'ls -lrt'
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