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
		withCredentials([usernamePassword(credentialsId: 'dockersecret', passwordVariable: 'dockerHubPassword', usernameVariable: 'dockerHubUser')]) {
        	sh "docker login -u ${env.dockerHubUser} -p ${env.dockerHubPassword}"
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
