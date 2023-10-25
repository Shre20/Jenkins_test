pipeline {
    agent any

    parameters {
        string(name: 'BUILD_VERSION', defaultValue: '1.0', description: 'Enter the build version')
        string(name: 'DEPLOY_ENV', defaultValue: 'DEVELOPMENT', description: 'Enter the deployment environment')
    }

    

    stages {
        stage('Build') {
            environment {
                BUILD_VERSION = "$params.BUILD_VERSION"
                DEPLOY_ENV = "$params.DEPLOY_ENV"
            }
            
            steps {
                sh 'echo "Building version ${BUILD_VERSION} for environment ${DEPLOY_ENV}"'
                // Add build steps here
            }
        }

        // Add more stages for deployment, testing, etc.
    }
}
