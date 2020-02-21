##############################
Instructions to run Dockerfile-1
##############################
1. You can create a docker file with different names it is not necessary to name it as "Dockerfile" always but when you do, you must explicitly mention the docker file name while building image.

example: docker build -t apacheimage -f ./dockerfileapache .
         name of image being created: apacheimage
         name of docker file: dockerfileapache
         directory where docker file is present: . (Current directory)
  
  docker run -d -p 80:80 -v /var/www/html:/var/www/html apacheimage
  when container is created, container contains apache pre installed and in running mode. 
  #########################################################################################
  
