pipeline {
    agent any
    environment{
        server_ip="${env.server_ip}"
    }
    
    stages {
        stage('Deploy') {
            steps {
                sh 'scp -r ${WORKSPACE}/* root@${env.server_ip}:"C:/inetpub/wwwroot/"'
            }
        }
    }
    
}

