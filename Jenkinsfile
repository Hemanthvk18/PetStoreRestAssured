pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the Git repository
                git 'https://github.com/Hemanthvk18/PetStoreRestAssured.git'
            }
        }

        stage('Build') {
            steps {
                script {
                    // Run Maven build
                    // Assuming Maven is installed on the Jenkins agent and the project has a pom.xml
                    sh 'mvn clean install'
                }
            }
        }
    }
}
