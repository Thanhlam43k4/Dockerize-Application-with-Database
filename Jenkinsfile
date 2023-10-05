pipeline{
    agent any
    stages{
        stage('Git Checkout'){
            steps{
                
                git 'https://github.com/Thanhlam43k4/Dockerize-Application-with-Database.git'
                echo 'Pulling code from Thanhlam43k4 GitHub'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing code from Thanhlam43k4 GitHub'
            }
        }
        stage('Build'){
            steps{
                sh 'docker compose build'
                sh 'docker compose up -d'
            }
        }
        stage('Push Image to Docker Hub'){
            steps{
                echo 'Pulling code from Thanhlam43k4 GitHub'
            }
        }
        stage('Deploy to K8S'){
            steps{
                echo 'Pulling code from Thanhlam43k4 GitHub'
            }
        }

    }
}
