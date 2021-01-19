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
        stage('testando script') {
            steps {
                sh './jenkins/scripts/delivery-for-production.sh'
            }
        }
    }

    stages {
        stage('Example') {
            steps {
                sh "./jenkins/scripts/delivery-for-development.sh"
            }
        }
    }
}
