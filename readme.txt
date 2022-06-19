Follow these steps to run the conatiner:


1.  Download the tar having the source code from this link:
    https://github.com/deepak-deez/ubuntu-nginx-image/blob/master/ubuntu_nginx.tar.gz

   



2. To extract the content of tar file
   $ tar -xzvf ubuntu_nginx.tar.gz 


3. build image from dockerfile using:
    docker build -t imagename:tag

4. Run this command to run the docker container:
   $  docker run -d -v myvol:/var/www/html --name={container_name} -p 80:80 {image_name:tag}

   myvol containing the index.html is present inside the tar file itself.

   The docker conatiner is up and running...!

   $. Use "curl localhost:80" to see the webpage content
      i.e curl 127.0.0.1:80



5. The Nginx access log & error log can be seen in the docker stdout & stderr using:
   $ docker logs {container_name}

6. We can get the client IP from these logs.