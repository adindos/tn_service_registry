pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Build tn_service_registry - pulling automatically'
            }
        }
        stage('Test') {
            steps {
                echo 'Test tn_service_registry - pulling automatically'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy tn_service_registry - pulling automatically'
            }
        }
    }
}
