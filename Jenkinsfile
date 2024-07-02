pipeline {
    agent any
    environment{
        server_ip="13.235.244.133"
    }
    
    stages {
        stage('Deploy') {
            steps {
                bat 'scp -r ${WORKSPACE}/* Administrator@13.235.244.133:/C:/inetpub/wwwroot/'
            }
        }
    }
    
}

