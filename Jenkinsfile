//Scripted syntax pipeline
/*node {
		echo "Build"
		echo "Test"
		echo "Integration Test"
		echo "one more test"
	}
*/

//Declarative
pipeline{
	//agent any
	agent { docker { image 'node:13.8' } }
	stages{
		stage('Build'){
			steps{	
				sh 'node --version'
				echo "Path - envi.$PATH"
				echo "build id - envi.$BUILD_ID"
				echo "build tag - envi.$BIULD_TAG"
				echo "job name - envi.$JOB_NAME"
				echo "Build id - envi.$BUILD_URL"
				
			}
		}
		stage('Test'){
			steps{
				echo 'testing'
			}
		}
		stage('integartion'){
			steps{
				echo 'integration testing'
			}
		}		
	}
	post{
		always{
				echo 'running always as am awesome'
		}
		success{
				echo 'I run when build when everything is right'
		}
		failure{
				echo 'I run when build fails and failure is stepping stone for success'
		}
	}
}