pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Run SonarQube Analysis') {
            steps {
                // Execute SonarQube scanner here
            }
        }

        stage('Publish to Artifactory') {
            steps {
                // Publish your artifacts to Artifactory here
            }
        }

        stage('Deploy') {
            steps {
                // Deploy your application (e.g., to a testing environment)
            }
        }
    }
}
