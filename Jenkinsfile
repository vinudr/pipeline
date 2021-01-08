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
		stage ('deploy'){
			parallel{
			stage ('deploy1'){
                	steps{
                	sh '''
                        echo "This is deployment 1 stage"
                        sleep 2
                   	'''
                	}
        		}
        	stage ('deploy2'){
                steps{
                	sh '''
                        echo "This is deployment 2 stage"
                        sleep 2
                   	'''
               		 }
		}
		}
		}
        stage ('test'){
                steps{
                sh '''
                        echo "This is test stage"
                        sleep 2
                   '''
                }
        }
}
}
