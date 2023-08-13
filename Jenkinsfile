pipeline
{
	agent any
	tools{
		maven "MAVEN_HOME"
	}
	stages{
		stage('Code Checkout'){
			steps{
				bat "echo checkout"
			}
		}
		stage('Code Test'){
			steps{
				bat "echo test"
			}
		}
		stage('Code Deploy'){
			steps{
				bat "echo deploy"
			}
		}
	}
	post{
		success{
			bat "echo success"
		}
	}
}
