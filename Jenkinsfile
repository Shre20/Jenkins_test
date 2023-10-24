pipeline { 
  agent any
  parameters {
      string (defaultValue: 'TEST', description: 'environment to deploy the application', name: 'ENV', trim: true)
      choice choices: ['main', 'Master'], description: 'Selecting available branch', name: 'BRANCH'
  }
  
  environment {
            DEPLOY_BRANCH = $BRANCH
            DEPLOY_ENV = $ENV
  }

  stages {
    stage ('BUILD') {
        steps {
            sh '''
                   echo Deploying to ${DEPLOY_ENV}
                   echo Code from ${DEPLOY_BRANCH} branch
                   exit 0
               '''   
        }
        
    }
  }
}