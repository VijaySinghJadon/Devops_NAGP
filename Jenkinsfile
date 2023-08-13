pipeline {
    agent any



    stages {
        stage('Checkout') {
            steps {
                bat "echo runt"
            }
        }

        stage('Build') {
            steps {
                   bat "mvn clean install"
                }
            }
        }

        // Add more stages as needed for testing, deployment, etc.
    }
}
