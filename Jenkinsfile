pipeline {
	agent {label 'master'}
	stages {
		stage ('build and deploy') {
		parallel {
		stage ('build') {
			steps {
			sh ' sleep 10 ; echo "this is build stage" '
			}
		}
		stage ('deploy') {
			steps {
			sh '''
			 sleep 10
			 echo "this is deploy stage"
			'''
			}
		}
		}
		}
		stage ('test') {
			steps {
			sh '''
			 sleep 10
			 echo "this is test stage"
			'''
			}
		}
	
	}
}
