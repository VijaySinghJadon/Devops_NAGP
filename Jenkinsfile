pipeline {
    agent any
        environment {
            notifyEmail="learntechjadon@gmail.com"
            }
    tools {
        maven 'maven_home'
        }

    stages {
        stage('code checkout') {
            steps {
                bat "echo hello"
                    }
            }

        stage('code build'){
            stpes{
                bat "mvn clean"
                    }
            }
            
        stage('unit test') {
            steps {
                bat "mvn test"
                }
            }

        stage('Run SonarQube Analysis') {
            steps {
                // Execute SonarQube scanner here
                }
            }
    }
}
