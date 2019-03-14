# Nginx Traffic Cone

Minimal Nginx config for local experiments: static site, JSON health endpoint, and a commented reverse-proxy example.

## Run

```bash
docker run --rm -p 8080:80 \
  -v "$PWD/nginx.conf:/etc/nginx/nginx.conf:ro" \
  -v "$PWD/html:/usr/share/nginx/html:ro" \
  nginx:1.25-alpine
```

Then open http://localhost:8080 and http://localhost:8080/api/health.

## License

MIT
