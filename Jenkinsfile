pipeline {
    agent { label 'slave'}

    stages {
            stage('Validade docker its running') {
            steps {
              sh '''
               docker info
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
            stage('Validade application its running') {
            steps {
              sh '''
               docker-compose top
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