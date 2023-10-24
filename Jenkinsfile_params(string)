pipeline { 
  agent any
  parameters {
      string (defaultValue: 'TEST', description: 'environment to deploy the application', name: 'ENV', trim: true)
      string (name: 'USERNAME', defaultValue: 'SHRE', description: 'Enter your username')
  }
  
  

  stages {
    stage ('ENV Stage') {
        steps {
         echo "Deploying to ${params.ENV}"
               
        }
        
    }
    stage('Username Stage') {
            steps {
                script {
                    def username = params.USERNAME
                    echo "Hello, ${username}! This is a user stage."
                }
            }
    }
  }
}