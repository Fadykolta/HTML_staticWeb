# HTML_staticWeb
docker run -d --name website  -p 8080:80 -v $PWD:/usr/share/nginx/html  nginx:latest