pipeline {
    agent any
          stages {
         
              stage('Change namespaces') {
                  steps {
                      
                      sh 'sudo sh namespace.sh $NAME $DOMAIN'
                  }
              }  
              stage('New port number') {
                  steps {
                      
                      sh 'sudo sh SG_Update.sh $PORTNUMBER'
                  }
              }   
           }
    
}
