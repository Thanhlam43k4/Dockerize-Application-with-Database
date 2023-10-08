pipeline{
    agent any
    stages{
        stage('Git Pulling Code'){
            steps{
                echo 'Pulling code from GitHub.....'
                git 'https://github.com/Thanhlam43k4/Dockerize-Application-with-Database-MySQL.git'
            }
        }
        
        stage('Build Docker image'){
            steps{
                sh 'docker build -t app_nodejs .' //Build app with image --name app_nodejs;
            }
        }
        stage('Testing'){
            steps{
                // sh 'npm install'
                // sh 'npm --version'
                // sh 'node --version'
                echo 'Testing stage .....'
            }
        }
        stage('Push Image to Docker Hub'){
            steps{
                withDockerRegistry(credentialsId: 'dockerhub_id', url: 'https://index.docker.io/v1/') {
                  sh 'docker build -t thanhlam2k4/nodejs_app .'
                  sh 'docker push thanhlam2k4/nodejs_app'
                }    
            }
        }
        stage('Run application in Local'){
            steps{
                // sh 'docker compose up'      //You can uncomment to run it on your local machine
            }
        }
        stage("Deploy to my Kubernetes Cluster Locally using Minikube"){
            steps{
                script{
                    kubernetesDeploy(configs: "deploymentservice.yml",kubeconfigId:"kubernetes")   //Something error because  K8scontinous deploy plugin was suspended
                }
            }
        }
    }
}
