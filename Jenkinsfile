pipeline {
    agent { label 'slave'}

    stages {
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