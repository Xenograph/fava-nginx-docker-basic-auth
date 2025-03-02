# Setup

1. `htpasswd -c ./nginx-config/htpasswd USERNAME`

2. `sudo docker compose run --rm certbot certonly --webroot --webroot-path /var/www/certbot/ -d YOUR_DOMAIN_NAME`

3. Edit `nginx-config/main.conf` and replace `YOUR_DOMAIN` everywhere

4. `sudo docker compose up -d`
