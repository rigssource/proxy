Reverse Proxy built on Nginx v1.0 
=================================================================================

docker-compose.yml – automation file that builds the solution from two docker files

proxy / docker file - builds nginx
web / docker file- build web server 
self signed certificates installed in proxy/certs folder
Port 80 is automatically forwarded to port 443 for authentication.

Run:
docker compose up -d --build

Top Secret Content: https://localhost/uj47G/index.html
Username: admin
Password: Password1
