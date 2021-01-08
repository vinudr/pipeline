pipeline{
	agent any
	stages{
	stage ('build'){
		steps{
		sh '''
			echo "This is build stage"
			sleep 2
		   '''
		}
	}
        	parallel {
		stage ('deploy1'){
	
                steps{
                sh '''
                        echo "This is build stage"
                        sleep 2
                   '''
                }
        }
        stage ('deploy2'){
                steps{
                sh '''
                        echo "This is build stage"
                        sleep 2
                   '''
                }
        }
	}
        stage ('test'){
                steps{
                sh '''
                        echo "This is build stage"
                        sleep 2
                   '''
                }
        }
} }
