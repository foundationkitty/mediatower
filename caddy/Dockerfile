FROM caddy:builder AS build

RUN xcaddy build --with="https://github.com/caddy-dns/cloudflare.git"

FROM caddy:latest

COPY --from=build /usr/bin/caddy /usr/bin/caddy
