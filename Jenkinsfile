pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking Out'
            }
        }
         stage('Package') {
            steps {
                bat 'mvn clean package'
            }
        }
        stage('JaCoCo Report') {
            steps {
                jacoco()
            }
        }
         stage('Build Docker Iamge') {
            steps {
               
            }
        }
         stage('Push Docker Image to Docker Hub') {
            steps {
              
            }
        }
        stage('Publishing') {
            steps {
                echo 'Publishing'
            }
        }
    }
}
