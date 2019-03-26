 1  docker build -t mynginx .  
 #this will build nginx and install curl into an image named 'mynginx'  
 2  docker run --name ngx -ti -d mynginx  
 #this will start your new image, put it in the background as the container named 'ngx'  
 3  docker exec -ti ngx /bin/bash  
 #this will connect to the container 'ngx' and run the shell command  
 #from here, execute:  curl -v  (you should get the curl version)  
 #exit the container with CTRL+C or exit   
 4  docker stop ngx  
 #this will stop the contianer  
 5  docker rm ngx  
 #this will remove the image from the process list    
