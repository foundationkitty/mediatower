FROM caddy:builder AS build

RUN xcaddy build --with=github.com/cadddy-dns/cloudflare

FROM caddy:latest

COPY --from=build /usr/bin/caddy /usr/bin/caddy
