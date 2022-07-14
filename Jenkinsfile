pipeline {
	agent any

stages { 
	stage('Checkout') { 
	   steps { 
		checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/devopsdeepdive/online-maven-project.git']]])
	   	}
    	}
    	stage('Validate') {
		steps { 
		 sh 'mvn validate'
		
		}
	}

    stage('Compile') {
		steps { 
		 sh 'mvn compile'
		
		}

	}
	stage('Test') {
		steps { 
		 sh 'mvn test'
		
		}

	}
	stage('Package') {
		steps { 
		 sh 'mvn package'
		
		}

	}
	}
}
    
