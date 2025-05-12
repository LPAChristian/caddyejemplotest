# Proyecto de EJEMPLO

git clone git@github.com:LPAChristian/caddyejemplotest.git

cd caddyejemplotest

Modificamos el archivo "Caddyfile" para poner el nombre del dominio real.
Nuestro dominio deberá de contener un wildcard (*) en las DNS.
Al ejecutarse, Caddy realiza un DNS-01 Challenge al dominio indicado.

Cuando se valida el certificado wildcard de manera automática este nos servirá para cualquier subdominio sin tocar cloudflare nunca más.

El certificado se guarda en "/data" y tiene validez de 90 días, Caddy lo auto-renueva.

docker-compose up -d --build

Las páginas de los subdominios se crean en la carpeta "site" con el formato {nombre}.{dominio}

