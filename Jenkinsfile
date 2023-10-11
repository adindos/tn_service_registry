pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Build tn_service_registry'
            }
        }
        stage('Test') {
            steps {
                echo 'Test tn_service_registry'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy tn_service_registry'
            }
        }
    }
}
