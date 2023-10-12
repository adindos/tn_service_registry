
// pipeline {
//     agent { docker {image 'maven : 3.9.2' } }
//     options {
//         // Timeout counter starts AFTER agent is allocated
//         timeout(time: 1, unit: 'SECONDS')
//     }
//     stages {
//         stage('Build') {
//             steps {
//                 script {
//                 // Build your Spring Boot application
//                 sh 'mvn clean package'
//                 }
//             }
//         }
//         stage('Test') {
//             steps {
//                 echo 'Test tn_service_registry - pulling automatically'
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 echo 'Deploy tn_service_registry - pulling automatically'
//             }
//         }
//     }
// }


node {
    // Define the Docker image you want to use as the build environment
    def dockerImage = 'maven:3.8.3-openjdk-11'

    // Checkout your source code from your version control system (e.g., Git)
    checkout scm

    // Run the build steps inside the Docker container
    docker.image(dockerImage).inside("-v ${env.WORKSPACE}:/workspace") {
        // Set the workspace inside the container
        def workspace = '/workspace'

        // Build your Maven project
        sh "cd ${workspace} && mvn clean package"
    }
}
