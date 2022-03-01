pipeline {
    agent { label 'slave'}

    stages {
        stage('Deploy application') {
            steps {
              sh '''
               docker-compose up -D
              ''' 
            }
        }
    }   
}