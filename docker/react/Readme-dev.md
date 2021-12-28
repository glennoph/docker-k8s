# docker react dev
## npm messages 
* need to upgrade nodejs

```
glenn@kubuntu-T3600:~$ sudo npm install -g create-react-app
sudo npm install -g create-react-app
[sudo] password for glenn: 
npm WARN deprecated tar@2.2.2: This version of tar is no longer supported, and will not receive security updates. Please upgrade asap.
/usr/local/bin/create-react-app -> /usr/local/lib/node_modules/create-react-app/index.js
npm WARN notsup Unsupported engine for create-react-app@5.0.0: wanted: {"node":">=14"} (current: {"node":"10.19.0","npm":"6.14.4"})
npm WARN notsup Not compatible with your version of node/npm: create-react-app@5.0.0
npm WARN notsup Unsupported engine for fs-extra@10.0.0: wanted: {"node":">=12"} (current: {"node":"10.19.0","npm":"6.14.4"})
npm WARN notsup Not compatible with your version of node/npm: fs-extra@10.0.0
```


## install npm v14

```
sudo apt update
curl -sL https://deb.nodesource.com/setup_14.x | sudo bash -
sudo apt-get install -y nodejs
node -v
# should see v14
sudo apt -y install gcc g++ make
curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update && sudo apt install yarn
yarn -V
# yarn install v1.22.17
sudo npm install -g create-react-app
node -v
# v14
```
## install project: frontend

cd docker/react
```
 create-react-app frontend
 
 ```
 * 3 commands to use:
 1. `npm run start` - set up dev server (not for prod)
 2. `npm run test`  - runs project test
 3. `npm run build `- builds production version of app
```

## Dockerfile
### Dockerfile.dev 
* for dev env
* cmd: `docker build -f Dockerfile.dev .`

#### React App Exits Immediately with Docker Run Command
3-22-2020

Due to a recent update in the Create React App library, we will need to change how we start our containers.

In the upcoming lecture, you'll need to add the -it flag to run the container in interactive mode:

`docker run -it -p 3000:3000 IMAGE_ID`


## docker-compose 
### up
cd 
