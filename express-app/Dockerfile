FROM node:16-alpine as build

COPY . .

RUN npm install --no-install-recommends && adduser -D user && rm -rf package-lock.json

USER user

CMD ["node", "index.js"]