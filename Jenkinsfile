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
               echo 'Building Docker Image'
            }
        }
         stage('Push Docker Image to Docker Hub') {
            steps {
              echo 'Pushing Docker Image'
            }
        }
        stage('Publishing') {
            steps {
                echo 'Publishing'
            }
        }
    }
}
