#### For PEM setup 
- To change permission since it won't allow if your key is public
```
chmod 400 ~/.ssh/bramk-backend_key.pem
```
https://bramk.southeastasia.cloudapp.azure.com:5050/test
https://bramk.southeastasia.cloudapp.azure.com:5050/test
### For Node and NPM

```
sudo apt update 
```

```
sudo apt install nodejs npm
```

**Install nvm**
```
curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
```

**Update to latest npm**
```
nvm install --latest-npm
```


### For nginx
```
sudo apt install nginx
```

```
sudo systemctl start nginx
```

```
sudo systemctl enable nginx
```

**Alow http requests**
```
sudo ufw allow 'Nginx HTTP'
```

	verify if it's working by visiting your public IP. You should be greeted by the NGINX screen

**SSL through certbot**
```
sudo certbot --nginx -d example.com
```


sample route where ssl is stored

	/etc/letsencrypt/live/bramk.southeastasia.cloudapp.azure.com/fullchain.pem
	/etc/letsencrypt/live/bramk.southeastasia.cloudapp.azure.com/privkey.pem


### Sample config to route / to :3000
so domain.com === localhost:3000
```
location / { 
	proxy_pass http://localhost:3000; # Your Express  
	proxy_http_version 1.1; proxy_set_header Upgrade $http_upgrade;
	proxy_set_header Connection 'upgrade';
	proxy_set_header Host $host;
	proxy_cache_bypass $http_upgrade; 
	}
```

### Setup github ssh
```
ssh-keygen -t rsa -b 4096 -C "andrewapinon@gmail.com"
```


When executed reload option the master Nginx process shuts down the child processes, loads the new configuration, and starts new child processes without disturbing operations. Hence, we prefer reload

```
sudo systemctl reload nginx
```