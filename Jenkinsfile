pipeline {
	agent any

    stages {
        stage ('Build') {
          steps {
			sh 'mvn --version'
			sh 'mvn clean install'
		 }
	   }

        stage ('Test') {
          steps {
			sh 'mvn test'
			ech 'Testing phase ...'
		 }
	   }

	}
   
   post {
		always {
			cleanWs()	
		}
	}
}
