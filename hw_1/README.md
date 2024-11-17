
Из папки hw_1:
```
 docker build -t my_nginx .
 docker run --name my_nginx_server -d -p 8081:80 my_nginx
```
Адрес сайта http://localhost:8081/