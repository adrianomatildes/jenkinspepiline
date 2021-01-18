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
        stage('Fazendo teste de scripts-2') {
            steps {
               sh 'whoami'
            }
        }
    }
}
