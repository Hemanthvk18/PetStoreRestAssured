pipeline {
    agent any
    stages {
        stage('Run Command') {
            steps {
                script {
                    if (isUnix()) {
                        // Unix command
                        sh 'nohup your-command &'
                    } else {
                        // Windows equivalent
                        bat 'start your-command'
                    }
                }
            }
        }
    }
}
