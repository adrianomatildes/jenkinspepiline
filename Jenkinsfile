pipeline {
    agent {
        docker {
            image 'node'
            args '-p 3000:3000'
        }
    }

    environment {
        CI = 'true'
    }
    stages {
        stage('Fazendo teste de scripts-1') {
            steps {
               sh './jenkins/scripts/test.sh'
            }
        }
    }
}
