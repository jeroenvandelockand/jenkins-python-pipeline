pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
		sh 'echo "Finished build"'
            }
        }
    }
}
post {
	always {
		echo 'This will always run'
	}
	success {
		echo 'This will run only if successful'
	}
	failure {
		echo 'This will run only if failed'
	}
}
