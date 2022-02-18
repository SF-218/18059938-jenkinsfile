pipeline {
	agent any
	stages {
		stage('Stage1 - 18059938'){
		steps {
			echo 'Stage 1 Completed - 18059938'
		}
		}
		stage('Stage2 - 18059938'){
		steps {
		 docker run -d -it -p 5000:80 --name=stage2-18059938-container -it apache2-18059938-image /bin/sh
		}
		}
		parallel {
			stage('Stage3 - 18059938') {
			steps {
				echo 'Stage 3 Completed - 18059938'
			}		
			}
			stage('Stage4 - 18059938') {
			steps {
				input('Proceed to release the work?')
			}
			}
			stage('Stage5 - 18059938') {
			when {
				not {
					branch "master executes"
				}
			}
			steps {
				echo 'Work Release - 18059938'
			}
			}
		}
	}

}
