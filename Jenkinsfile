pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Construindo teste de instalando nodes') {
            steps {
                sh 'npm install'
            }
        }
    }
}
