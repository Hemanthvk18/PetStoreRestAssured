pipeline {
    agent any

    tools {
        maven 'Maven 3'  // This should match the Maven installation you configured in Jenkins
    }

    environment {
        JAVA_HOME = 'C:/Program Files/Java/jdk-21'
    }

    stages {
        stage('Build') {
            steps {
                script {
                    // Running the Maven clean install command
                    bat "mvn clean install"
                }
            }
        }

        stage('Package') {
            steps {
                script {
                    // Running the Maven clean package command
                    bat "mvn clean package"
                }
            }
        }
    }
}
