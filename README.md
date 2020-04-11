# Phalcon Docker Compose

Phalcon 4.0.5 + PHP7.4


 1. Run: `docker-compose up -d`

 2. docker-compose.yml - You can add service here. such as memcached-server , phpmyadmin , etc.

 3. variables.env - This file use to define the environment variable of service.

 **Note : You have to look the variable in your image. eg. [mysql-docker][:mysql-docker:] (Environment Variables Section)**

 4. application folder - This folder is the directory of your project.

 5. Use docker run command to use and mount volume to your project
    ex: `docker run --name phalcon -d -p 1000:80 -v /Users/chipv/Desktop/phalcon/phalcon-docker/application:/var/www/html phalcon-docker` 

 6. Reference

[:phalcon:]:        https://github.com/phalcon/cphalcon
[:docker:]:         https://www.docker.com
[:phalcon-version:]:  https://github.com/phalcon/cphalcon/releases
[:mysql-docker:]:   https://hub.docker.com/_/mysql
