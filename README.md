 
 # below command will run the image if exist else pull the latest image of mysql it will run on port 3306 -d will run it in detatched mode
 

 docker run -d --name mysqldb -p 3306:3306 -e MYSQL_ROOT_PASSWORD=password mysql:latest
 

#run the below command to list the container
 docker ps
 
 #run the image
 docker run exec -it mysqldb bash
 
 #on bash run the below command to login note -p need to appended to "password"
  mysql -u root -ppassword 


# to get IPAddress
docker port $imagename  


#grep command
docker inspect mysql | grep IPAdress

 
 
 
 
