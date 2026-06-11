*Laboratorium 13 Docker Compose*
Autor: Aleksandra Grzywacz

Użyte polecenia:

1. Przygotowanie struktury plików:

mkdir -p www
<br>
echo "<?php phpinfo(); ?>" > www/index.php
<br>
mkdir -p nginx/conf.d

<img width="694" height="140" alt="image" src="https://github.com/user-attachments/assets/ed15c52b-5ef7-40b9-8db0-6ab41ef41b5c" />
<br>
<img width="206" height="603" alt="image" src="https://github.com/user-attachments/assets/0897053b-deaa-4d61-8f55-2beb09af595b" />


2. Uruchomienie Docker Compose

docker compose up -d
<img width="957" height="342" alt="image" src="https://github.com/user-attachments/assets/05a9deb1-1742-478c-8ef5-7354ff3bcb6f" />


3. Weryfikacja działania

curl localhost:4001

<img width="957" height="490" alt="image" src="https://github.com/user-attachments/assets/9e0bbcb2-8475-4961-bad8-893d50ca4305" />

<br>
<img width="1919" height="772" alt="image" src="https://github.com/user-attachments/assets/667f44f8-3f5b-48ec-8d61-e3f1041209bb" />
jak widać na zrzucie ekranu utworzona została baza testdb oraz udało się zainicjować też bazę nowabazka

4. Uzasadnienie
Kontener phpMyAdmin podłączyłam zarówno do sieci backend jak i frontend. Musiał zostać podłączony do backend, ponieważ inaczej nie mógłby komunikować sie z serwerem bazy danych, która tam się znajduje, aby chronić ją przed bezpośrednim dostępem ze świata zewnętrznego. Podłączyłam go również do frontend, ponieważ posiada interfejs graficzny, do którego potrzebny jest bezpośredni dostęp z poziomu przeglądarki.
