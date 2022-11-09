
### NGINX PHP-FPM MYSQL

Run the dockers manually

```bash
docker run -itd -p 80:80 -v socket:/var/run/php/ -v docroot:/var/www/html/  nginx:v1
docker run -itd -v socket:/var/run/php/ -v docroot:/var/www/html/:ro fpm:v1

