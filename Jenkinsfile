pipeline {
    agent { label 'slave'}

    stages {
            stage('Validade docker it's running') {
            steps {
              sh '''
               docker-compose up -d
              ''' 
              }
            }
           stage('Deploy application') {
            steps {
              sh '''
               docker-compose up -d
              ''' 
            }
        }
        stage('Stop application') {
            steps {
              sh '''
               docker-compose stop
              ''' 
            }
        }
    }   
}