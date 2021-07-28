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
	post{
		always{
				echo 'I am running always'
		}
		success{
				echo 'I run when build is successful'
		}
		failure{
				echo 'I run when build fails'
		}
	}
}