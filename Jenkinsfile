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
	agent any
	stages{
		stage('Build'){
			steps{
				echo 'Building'
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
}