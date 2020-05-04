pipeline {
	agent any

    stages {

        stage ('Build') {
          steps {
			sh 'mvn --version'
			sh 'mvn clean compile'
		 }
	   }

        stage ('Test') {
          steps {
			sh 'mvn test'
		 }
	   }

	}
   
   post {
		always {
			cleanWs()	
		}
	}
}
