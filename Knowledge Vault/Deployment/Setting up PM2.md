SERVER:  
```
pm2 start ./build/server.js --name tm-chateasy-server
```


CLIENT  
`NODE_ENV=production pm2 start ./src/server.js --interpreter ./node_modules/@babel/node/bin/babel-node.js --name tm-chateasy-client`


ssh-keygen -t rsa -b 4096 -C "andrewapinon@gmail.com"


ssh -i ~/.ssh/andrew.pem andrew@172.188.49.40


pm2 start ./server/src/server.js --name ai