pipeline {
	agent any 
	stages {
		stage('Both build and test') {
			parallel {
				stage('Build') { 
					steps {
						sh 'sleep 15; echo "This is a Build stage"'
					}
				}
				
				stage('Test'){
					steps {
						sh '''
							sleep 15
							echo "This is a Test stage"
						'''	
				
					}
            
                        
                    }
				}
                stage('test1'){
                    steps{
                        sh '''
                            echo "this is test1"
                        '''

                    }
                }
			} 
		}
		stage('Deploy'){
			steps {
				sh '''
					sleep 5
					echo "This is a Deploy stage"
				'''
			}
		}
		
		stage('My-stage'){
			steps {
				sh '''
					sleep 5
					echo "This is a My-stage stage"
				'''
			}
		}	

	}
}