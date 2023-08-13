pipeline{
    agent any
        environment {
        notifyEmail ="vijay.jadon@nagarro.com"
    }
    tools{
        maven 'maven_home'
    }
    triggers {
        cron('0 07 * * *')
      }
    stages{
        stage("code checkout"){
            steps{
            bat "echo hello"
            }
        }   

 

        stage("code build"){
            steps{
             bat "mvn clean test"
            }
        }
        stage("unit test"){
            steps{
            bat "mvn test "
            }
        }
    }
    post{
        success{
            bat "echo success"
            }
        }
}
