pipeline {
	agent any
	stages {
		stage('Stage1 - 18059938'){
		steps {
			echo 'Stage 1 Completed - 18059938'
		}
		}
		stage('Stage2 - 18059938'){
		docker {
			image 'apache2-18059938-image:latest'
			reuseNode true
		}
		steps {
		sh 'apache2-18059938-image --version'
		sh 'docker run -d --name=stage2-18059938-container -it apache2-18059938-image .'
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
