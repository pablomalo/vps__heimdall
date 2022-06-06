# vps__heimdall

A dashboard for all your web applications. See https://github.com/linuxserver/Heimdall

## Installation

1. Copy `.env.dist` to `.env` and set relevant environment variables, with particular attention to those commented with "TODO Set me".

2. `docker-compose up -d`

3. Run the following commands for the app name to be picked up.
   ```
   docker compose exec -it heimdall php /var/www/localhost/heimdall/artisan
   docker compose exec -it heimdall php /var/www/localhost/heimdall/artisan config:clear
   ```