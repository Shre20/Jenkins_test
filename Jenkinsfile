pipeline { 
  agent any
  parameters {
      string defaultValue: 'TEST', description: 'environment to deploy the application', name: 'ENV', trim: true
  }

  
  stages {
    stage ('BUILD') {
        steps {
            sh '''
            echo Deploying to ${params.ENV}
            exit 0
            '''
        }
        
    }

  }
}