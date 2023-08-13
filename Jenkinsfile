pipeline {
    agent any

    tools {
        // Specify the 'Maven' tool by name
        maven 'Maven 3.9.4' // The name of the Maven installation in Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                script {
                    // Retrieve the Maven installation path
                    def mvnHome = tool name: 'Maven 3.8.3', type: 'hudson.tasks.Maven$MavenInstallation'
                    // Use Maven to build the project using batch script
                    bat "${mvnHome}\\bin\\mvn clean install"
                }
            }
        }

        // Add more stages as needed for testing, deployment, etc.
    }
}
