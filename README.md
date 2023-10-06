# Dockerize-Application-with-Database MySQL



        Dockerize Web application with docker 

--Prequesites:


+ Nodejs web application and MySQL Database (Dependencies: Express, Mysql2).
+ Download Docker, Docker-compose, DockerFile.
+ PHPMYADMIN to managing MYSQL and MariaDB databases.

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



  >>This is a simple project for you to can start with your Devops RoadMap.


