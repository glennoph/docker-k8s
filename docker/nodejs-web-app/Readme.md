# docker nodejs web app

## build

 docker login
 # enter userid, pw
 
 docker build  -t gomn/nodejsweb .

## run

 docker run -p 8080:8080 gomn/nodejsweb