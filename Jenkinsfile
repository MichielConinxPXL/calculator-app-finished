pipeline {
    agent any
   
    stages {
        stage('opdracht 5') {
            steps {
                echo "good luck..."
            }
        }
        stage('checkout code') {
            steps {
            	 git branch:'main', credentialsId:'77f29521-2102-44a4-af52-cdaec526dddf', url:'https://github.com/TomWillenPXL/calculator-app-finished.git'
            }
        }
        stage('install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('unit test'){
            steps {
                sh 'npm test 2>output.txt'
            }
        }
        
    }
}
