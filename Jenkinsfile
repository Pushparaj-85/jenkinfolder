pipeline {
    agent any
    tools {nodejs "mynodejs"}
    stages {
        stage('UAT') {
            steps {
                git credentialsId: 'webhookserver', url: 'https://github.com/Pushparaj-85/jenkinfolder.git'
                sh '''echo "This is a new pipeline"
            }
        }
        stage ('DEV') {
            steps {
            sh 'npm install'    
            }
        }
    }
}
