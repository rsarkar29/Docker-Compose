# Docker Compose for local Development

## setup
1. clone the repo

```
```
2. Place your mysqldump to ./docker-utlis/app/ directory.
3. From root Run below command

```
docker-compose up --build -d
```
4. Now check both the container running or not

```
docker ps
```
It should be like this

![alt text](https://tecadmin.net/tutorial/wp-content/uploads/2017/09/docker-ps-command.png)


5. Now Go to web_db conatiner using below command
```
docker exec -it <container-id> bash
```
6. go to app directory and import the dump

```
mysql -u drupal -p drupal < cityguide.sql
```
7. Go to localhost:8099
 
