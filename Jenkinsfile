pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
               git credentialsId: '6a466836-8697-41a3-b2ae-06c69062b2bf', url: 'https://github.com/bunnyyar/saikumar.git'
            }
        }
        
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        
        stage('Build') {
            steps 
                sh 'npm run build'
            }
        }
    }
}
