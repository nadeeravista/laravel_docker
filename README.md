## Overview
This repository is a docker project. The Nginx is the web server and Mysql is the database management system

## Folder description or as specify in the docker-compose.yml

./src
The Leravel applcaiton code. or specify the code base location

./data
Docker volumes for mysql is linking with these directory - Persistant data store

./nginx
Seetings for Nginx server running on docker.


## Installation steps

### Prereqeusts
You need following packages for installing the application
Git - for downloading the reporsitory
Docker Desktop - All the application will start here


Clone or download the code to any location

```
....
  php:
   ...
    volumes: 
      - ./src:/var/www/html // A location inside docker folder or outside. ./src is host location
    ....
```

### Starting up services
```
docker-compose build && docker-compose up -d
```

