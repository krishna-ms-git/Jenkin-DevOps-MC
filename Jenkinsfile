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
			step{
				echo 'Building'
			}
		}
		stage('Test'){
			step{
				echo 'testing'
			}
		}
		stage('Build'){
			step{
				echo 'Building'
			}
		}		
		}
}