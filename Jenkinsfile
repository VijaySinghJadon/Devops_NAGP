pipeline {
    agent any

    tools {
        // Define the 'Maven' tool by name
        maven 'Maven' // The name specified in Jenkins configuration
    }

    stages {
        stage('Checkout') {
            steps {
                bat "echo checkout"
            }
        }

        stage('Build') {
            steps {
                script {
                    def mvnHome = tool name: 'Maven', type: 'hudson.tasks.Maven$MavenInstallation'
                    sh "${mvnHome}/bin/mvn clean install"
                }
            }
        }

        // Add more stages as needed for testing, deployment, etc.
    }
}
