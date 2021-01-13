pipeline {
    agent any

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
