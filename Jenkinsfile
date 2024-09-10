pipeline {
    agent any
    tools {nodejs "mynodejs"}
    stages {
        stage('master') {
            steps {
                git credentialsId: 'webhookserver', url: 'https://github.com/Pushparaj-85/jenkinfolder.git'
                echo " file content is "
            }
        }
        stage ('build') {
            steps {
            sh 'npm install'    
            }
        }
    }
}
