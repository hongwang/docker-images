FROM node:14-alpine

RUN apk add --no-cache --virtual .build-deps-pnpm curl \
    && curl -f https://get.pnpm.io/v6.16.js | node - add --global pnpm \
    && apk del .build-deps-pnpm \
    && pnpm --version
