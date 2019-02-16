# Nginx Traffic Cone

Tiny **reverse-proxy + static site** demo for first meetings with Nginx.

```bash
docker run --rm -p 8080:80 \
  -v "$PWD/nginx.conf:/etc/nginx/nginx.conf:ro" \
  -v "$PWD/html:/usr/share/nginx/html:ro" \
  nginx:1.25-alpine
```

Backend/infra practice · serious config · unserious name.

MIT · 2019
