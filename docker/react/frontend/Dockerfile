# Dockerfile for prod

FROM node:16-alpine as builder

workdir /app
copy package.json .
run  npm install
copy . .

run npm run build

# nginx
from nginx
copy --from=builder /app/build /usr/share/nginx/html

