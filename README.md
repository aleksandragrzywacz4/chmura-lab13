*Laboratorium 13 Docker Compose*
Autor: Aleksandra Grzywacz

Użyte polecenia:

1. Przygotowanie struktury plików:

mkdir -p www
echo "<?php phpinfo(); ?>" > www/index.php
mkdir -p nginx/conf.d

<img width="694" height="140" alt="image" src="https://github.com/user-attachments/assets/ed15c52b-5ef7-40b9-8db0-6ab41ef41b5c" />
<br>
<img width="206" height="603" alt="image" src="https://github.com/user-attachments/assets/0897053b-deaa-4d61-8f55-2beb09af595b" />


2. Uruchomienie Docker Compose

docker compose up -d
<img width="957" height="342" alt="image" src="https://github.com/user-attachments/assets/05a9deb1-1742-478c-8ef5-7354ff3bcb6f" />


3. Weryfikacja działania

curl localhost:4001

<img width="951" height="508" alt="image" src="https://github.com/user-attachments/assets/4c2d6b88-2136-4506-a2af-c42dfd14ba2e" />

<img width="1895" height="787" alt="image" src="https://github.com/user-attachments/assets/c9c22f4e-22e0-4e43-9633-d8846861474a" />

