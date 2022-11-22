pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
		sh 'docker build -t nginx-docker .'
		
                // 
            }
        }
        stage('Test') { 
            steps {
		sh 'echo Skip'
                // 
            }
        }
        stage('Deploy') { 
            steps {
		sh 'echo Skip'
                // 
            }
        }
    }
}
