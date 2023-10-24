pipeline {
  
  stages {

    stage ('BUILD') {
      agent any
      steps {
        echo "This is Build stage" 
        sh ''' 
		sleep 5
	        exit 0 
	   '''
      }  
    }  
    
    stage ('TEST') {
      agent { label 'Shre-slave1' }
      steps {
        echo "This is Test stage" 
        sh 'sleep 5'
      }  
    }  
    
    stage ('DEPLOY') {
      agent { label 'Shre-slave1' }
      steps {
        echo "This is Deploy stage" 
        sh 'sleep 5'
      }  
    }  
  } 

}