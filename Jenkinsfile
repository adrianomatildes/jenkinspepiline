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
               sh './jenkins/scripts/test.sh'
            }
        }
    }
}
