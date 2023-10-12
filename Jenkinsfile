
pipeline {
    agent { docker {image 'maven : 3.9.2' } }
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                script {
                // Build your Spring Boot application
                sh 'mvn clean package'
                }
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
