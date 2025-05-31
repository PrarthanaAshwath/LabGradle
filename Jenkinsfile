pipeline
{
	agent any
	tools{
		gradle:'gradle'
		jdk:'jdk'
	}
	stages{
		stage('Checkout')
		{
			steps{
				git "https://github.com/PrarthanaAshwath/LabGradle.git"
			}
		}
		stage('Build')
		{
			steps{
				sh 'gradle build'			
			}
		}
		stage('Test')
		{
			steps{
		                sh'gradle test'
		        }
		}
		stage('Run-Application')
		{
			steps{
				sh 'gradle run'			
			}
		}
		
	}
}

