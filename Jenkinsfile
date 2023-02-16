pipeline {
 agent any
	 stages {
		 stage('Build') {
		 steps {
			 sh 'g++ -o PES2UG20CS371-1 ./new.cpp'
			 echo 'Build stage has been completed successfully'
		 }
	 	}
		 stage('Test') {
			 steps {
			 ph './PES2UG20CS371-1'
			 echo 'Testing stage has been completed successfully'
			 }
		 }
		 stage('Deploy') {
			 steps {
			 echo echo 'Deploying stage has been completed successfuly'
			 }
		 }
	}
	post {
		failure {
		 	echo 'Pipeline failed'
		 }
	 }
}
