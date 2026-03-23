pipeline {
    agent any
    
    tools {
        // These names must match what you configured in Global Tool Configuration
        maven "MAVEN1" 
    }

    stages {
        stage('Checkout') {
            steps {
               checkout scm
            }
        }
        
        stage('Build') {
            steps {
                // We removed the 'dir' block because Jenkins is already 
                // inside your workspace folder by default.
                bat 'mvn clean compile'
            }
        }
        stage('Test') {
            steps {
                // We removed the 'dir' block because Jenkins is already 
                // inside your workspace folder by default.
                bat 'mvn test'
    }
    
  
            
        }
    

