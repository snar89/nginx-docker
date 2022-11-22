pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
		sh 'docker build -t snaredla89/p1:latest .'
		
                // 
            }
        }
        stage('Push') { 
            steps {
		sh 'docker login -u snaredla89 -p Welcome2docker'
          	sh 'docker push snaredla89/p1:latest'
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
