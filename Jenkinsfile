pipeline {

    agent any

    stages {
    
        stage('git checkout') {
        
            steps {
                echo 'building the application' 
            }
        }
        
         stage('sonar scanner') {
        
            steps {
                echo 'testing the application' 
            }
        }
        
         stage('docker build and tag') {
        
            steps {
                sh 'docker build ./ -t image:tag'
                
            }
        }
    }
}
