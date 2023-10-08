# Dockerize-Application-with-Database MySQL And Continuous Integration by Jenkins



        Dockerize Web application with docker 

--Prequesites:


+ Nodejs web application and MySQL Database (Dependencies: Express, Mysql2).
+ Download Docker, Docker-compose, DockerFile.
+ PHPMYADMIN to managing MYSQL and MariaDB databases.
+ DockerHub account

STEPS:

  STEP1: Clone this repository .

            git clone https://github.com/Thanhlam43k4/Dockerize-Application-with-Database.git
 
  STEP2: Run this server using docker-compose.

            docker compose up -d 

  STEP3: Connect your application on the web browser.

            localhost:8080

        Connect to your Database

            localhost:8080/connect

  STEP4: You can manage your data in PHPMYADMIN (with user:thanhlam password: secret).

          localhost:8081

  STEP5: Search localhost:8081/fetch you can see your data in table "mytable" in Database "mydb".



 ** Use Jenkins Pipeline to Continuous Integration.**
  These are Steps in Jenkins Pipeline:

 + Step1 : Pulling Code From Github

 + Step2 : Build Docker image with name app_nodejs in this dir //You can change

 + Step3 : Testing application (I'll update soon)

 + Step4 : Push This image to your DockerHub (In my case I push to my Dockerhub account, you must change it)

 + Step5 : You can run application in your local computer use "docker compose up"

 + Step 6: Deploy to K8s local (I'll update it soon).

   > SuccessFully Set up and Start to use your application !!!!

  >>This is a simple project for you to can start with your Devops RoadMap.



Author: NguyenThanhlam K67K2UET


