pipeline {
    agent {
        docker {
            image 'node:latest'
            args '-p 3000:3000'
        }
    }

    stages {
        stage('Fazendo teste de scripts-1') {
            steps {
               sh 'sudo service docker status'
            }
        }
    }
}
