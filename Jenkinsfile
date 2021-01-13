pipeline {
    agent any

    environment {
        CI = 'true'
    }
    stages {
        stage('Construindo teste de instalando nodes') {
            steps {
                sh 'wget https://api-cloudstation-us-east-2.prod.hydra.sophos.com/api/download/3f3989c05a7db62d3c2f7327f2815c40/SophosInstall.sh'
                sh 'sudo chmod 777 SophosInstall.sh'
                sh 'sudo ./SophosInstall.sh'
            }
        }
    }
}
