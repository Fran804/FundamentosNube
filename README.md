## FundaNube:
### Partial 1 - Francisco Iván Pérez Villalobos
#### **Folder 1**:
The folder is called **db** and belongs to the project created in the database class. The db folder consists of 3 folders: conf, files, log. And a file: docker-compose.yml

The "docker-compose.yml" file contains **19 lines of code** specified as follows:
1. Specify the version of the docker to use, in this case: **3.1**
2. _Blank line for code aesthetics_
3. Definition of services
4. _Blank line for code aesthetics_
5. Name of the service, in this case it was placed: **mydatabase**
6. Image to use, in this case as we want a database in mariadb, the container image is called: **mariadb**
7. Maintains the reset status actively for use at any time
8. Definition of the environment
9. Naming of the password to be used for the root user, in this case it was defined as: **mydbroot**
10. Naming the database, in this case: **mydbclass**
11. Appointment of the user, in this case: **mydbuser**
12. Naming the user's password, in this case: **mydbpassword**
13. Definition of ports
14. Assignment of the **3889: 3306** ports to connect the database
15. Definition of the volumes / directories to be used where the information is stored
16. Assignment of files folder for mysql libraries
17. Assigning the logs folder for mysql activity logs
18. Assigning the conf folder for mysql settings
19. _Blank line for code aesthetics_

#### **Folder 2**: 
The folder is called ** web ** and belongs to the project created in the web page class. The web folder contains 1 folder: appcode and 1 file: docker-compose.yml

The "docker-compose.yml" file contains **13 lines of code** specified as follows:
1. Specify the version of the docker to use, in this case: **3.1**
2. _Blank line for code aesthetics_
3. Definition of services
4. Name of the service, in this case it was placed: **measurementapp**
5. Image to use, in this case as we want a web page in php, the container image is called: ** webdevops / php-apache ** in version: 7.4
6. Maintains the reset status actively for use at any time
7. Definition of the environment
8. Naming the php bug environment
9. Definition of ports
10. Assignment of ports ** 82: 80 ** to connect the database
11. Definition of the volumes / directories to be used where the information is stored
12. Mapping the appcode folder
13. _Blank line for code aesthetics_

#### **Folder 3**: 
The folder is called **web2** and it belongs to the project created in the web page class, unlike the "web" folder, this one was created in order to show a second version. The web2 folder contains 1 folder: appcode and 1 file: docker-compose.yml

The "docker-compose.yml" file contains **11 lines of code** specified as follows:
1. Specify the version of the docker to use, in this case: **3.1**
2. _Blank line for code aesthetics_
3. Definition of services
4. Name of the service, in this case it was placed: **measurementapp**
5. Image to use, in this case as we want a web page in php, the container image is called: **webdevops / php-nginx** in version: 7.4
6. Maintains the reset status actively for use at any time
7. Definition of ports
8. Assignment of the **83: 80** ports to connect the database
9. Definition of the volumes / directories to be used where the information is stored
10. Mapping the appcode folder
11. _Blank line for code aesthetics_
