# docker react

## docker react prod
See [Readme-dev.md](Readme-dev)

## docker react prod
### dockerfile

See [Dockerfile](./frontend/Dockerfile)

* from node:16-alpine as builder
create /app/build dir

* from nginx
copy from builder /app/build to /usr/share/nginx/html

## build 
`docker build .`
* copy sha from : Successfully build (sha)

## run
`docker run -p 8080:80 (sha)`
sha from build (above)

### browser 
[localhost:8080](http://localhost:8080)

