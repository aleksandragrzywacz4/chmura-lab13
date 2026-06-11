*Laboratorium 13 Docker Compose*
Autor: Aleksandra Grzywacz

Użyte polecenia:

1. Przygotowanie struktury plików:

mkdir -p www
echo "<?php phpinfo(); ?>" > www/index.php
mkdir -p nginx/conf.d


2. Uruchomienie Docker Compose

docker compose up -d


3. Weryfikacja działania

curl localhost:4001

