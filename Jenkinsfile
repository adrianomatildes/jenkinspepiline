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
        stage('testando o deployament') {
            sh './jenkins/scripts/deliver-for-development.sh'
        }
    }
    stages {
        stage('Fazendo teste de scripts-4') {
            steps {
               sh './jenkins/scripts/test.sh'
            }
        }
    }

}
