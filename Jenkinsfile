pipeline {
    agent {
        docker {
            image 'node:14.15.4'
            args '-p 3000:3000'
        }
    }

    environment {
        CI = 'true'
    }
    stages {
        stage('testando o teste de deliver-for-development') {
            steps {
                sh './jenkins/scripts/delivery-for-development.sh'
            }
        }
    }
    stages {
        stage('testando o teste de deliver-for-production.sh') {
            steps {
                sh './jenkins/scripts/delivery-for-production.sh'
            }
        }
    }
    
    stages {
        stage('Fazendo teste de scripts-delivery') {
            steps {
               sh './jenkins/scripts/test.sh'
            }
        }
    }
}
