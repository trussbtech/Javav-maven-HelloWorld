node {
    stage('SCM') {
		echo 'Gathering code from version control'
		git branch: '${branch}', url: 'https://github.com/trussbtech/sample_android_app-java.git'
    }
    stage('Build') {
		echo 'Building....'
		sh 'mvn --version'
		sh 'mnv clean
		sh 'mvn compile'
	}	
    stage('Test') {
		echo 'Testing At master branch'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}