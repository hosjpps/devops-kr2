# KR2: Flask + Redis behind Nginx

Variant 1: `https://api.devops.local`, application port `8001`.

Server: `~/kr2` on `devops-vm`, Nginx site `/etc/nginx/sites-available/kr2` (copy in `nginx/kr2`).

```bash
cp .env.example .env    # on the server: REDIS_PASSWORD=$(openssl rand -hex 32), chmod 600
docker compose up -d --build
```
