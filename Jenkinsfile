pipeline {
    agent { docker { image 'maven:3.9.4-eclipse-temurin-17-alpine' } }
    stages {
        stage('build') {
            steps {
                echo 'Deploy tn_service_registry build automatically #15'
                sh 'mvn --version'
            }
        }
    }
}
