# HTML_staticWeb
docker run -d --name website  -p 8080:80 -v $PWD:/usr/share/nginx/html  nginx:latest

Here is what each of the options in the command do:

-d: runs the container in detached mode, meaning it will run in the background and not attach to the terminal

--name website: sets the name of the container to "website"

-p 8080:80: maps port 8080 on the host machine to port 80 on the container. This means that when you access port 8080 on the host machine, it will be forwarded to port 80 in the container.

-v $PWD:/usr/share/nginx/html: mounts the current working directory ($PWD) on the host machine to the /usr/share/nginx/html directory in the container. This is where Nginx looks for the HTML files it serves.

nginx:latest: specifies the image to use for the container, which is the latest version of the official Nginx image available on Docker Hub.


