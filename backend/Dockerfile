from node:20
workdir /app
copy package.json .
copy *.js .
run npm install
env DB_HOST=mysql
cmd ["node" , "index.js"]