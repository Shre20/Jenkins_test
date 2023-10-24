pipeline { 
  agent any
  parameters {
      string defaultValue: 'TEST', description: 'environment to deploy the application', name: 'ENV', trim: true
  }

  stages {
    stage ('BUILD') {
        steps {
         echo "Deploying to ${params.ENV}"
               
        }
        
    }

  }
}