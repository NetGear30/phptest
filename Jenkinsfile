pipeline {
    agent any
    environment{
        server_ip="13.235.244.133"
    }
    
    stages {
        stage('Deploy') {
            steps {
                bat 'scp -r ${WORKSPACE}/* Administrator@${server_ip}:/C:/inetpub/wwwroot/'
            }
        }
    }
    
}

