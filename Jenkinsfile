pipeline {
    agent { label 'slave01'}

    stages {
        stage('Deploy application') {
            steps {
              sh '''
               docker --version
              ''' 
            }
        }
    }   
}