create dockerfile
FROM  amazonlinux
RUN   yum update
RUN   yum install httpd -y
COPY  index.html  /var/www/html/
EXPOSE 80
CMD   ["httpd", "-D", "FOREGROUND"]
build docker image
docker build -t image-1 .
or

docker build -t abhipraydh96/img-1 .
