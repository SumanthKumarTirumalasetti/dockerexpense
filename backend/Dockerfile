# from node:20
from node:20.18.3-alpine3.21
RUN addgroup -S expense && adduser -S expense -G expense
run mkdir /opt/backend
run chown -R expense:expense /opt/backend
workdir /opt/backend
copy package.json .
copy *.js .
run npm install
env DB_HOST=mysql
user expense
cmd ["node" , "index.js"]