TODO:

```shell
sudo docker run -it --name caddy \
  -p 80:80 \
  -p 443:443 \
  -v caddy_data:/data \
  -v caddy_config:/config \
  -v $PWD/Caddyfile:/etc/caddy/Caddyfile \
  -e CLOUDFLARE_EMAIL=me@example.com \
  -e CLOUDFLARE_API_TOKEN=12345 \
  -e ACME_AGREE=true \
  image/imageName
```
