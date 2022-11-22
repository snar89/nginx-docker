pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
		sh 'docker build -t nginx-docker .'
		
                // 
            }
        }
        stage('Push') { 
            steps {
		sh 'docker push snaredla89/p1:nginx-docker'
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
