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
        stage('Fazendo teste de scripts') {
            steps {
               sh './jenkins/scripts/test.sh'
            }
        }
    }
}
