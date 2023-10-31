pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository
                checkout scm
            }
        }
        
        stage('Build') {
            when {
                // Define conditions for 'master' branch execution
                expression { return env.BRANCH_NAME == 'master' }
            }
            steps {
                // Your build steps here
                sh 'echo "Building on master branch"'
                // Add your build commands or scripts
            }
        }
    }
}