
RUN OUTSIDE SSH 
<p style="font-size:0.9rem; color:grey;">run the commands in your local terminal. Do not ssh into the server you want to download/upload files from or to.</p>

TO DOWNLOAD FROM SERVER
```` bash
scp -r -i ~/.ssh/tm-andrew james@206.189.168.89:~/dump/tm-chateasy ~/Desktop/devDump
````

  
_UPLOAD TO SERVER  
``` bash
scp -r -i ~/.ssh/tm-andrew ~/Desktop/devDump/tm-chateasy james@206.189.168.89:~/dump/
```



Command stripped with generic placeholders

DOWNLOADING FROM SERVER
```bash
scp -r -i dir/of/ssh_key username@ipaddress:dir/of/file/in/server dir/of/local
```




Get error logs from production server ChatEasy
```
scp -r -i ~/.ssh/tm-andrew azureuser@20.120.19.74:/home/azureuser/.pm2/logs/tm-chateasy-server-0-error.log ~/Desktop/devDump
```

Get error logs from production RabbitMQ

```bash
scp -r -i ~/.ssh/tm-andrew azureuser@20.85.219.225:/var/log/rabbitmq/rabbit@TMRabbitMQ0.log ~/Desktop/devDump
```

scp -r -i ~/.ssh/tm-andrew ~/Desktop/devDump/tm-chateasy james@178.128.76.4:~/dump/

[james@178.128.76.4](mailto:james@178.128.76.4)

scp -r -i ~/.ssh/tm-andrew azureuser@20.127.14.169:/var/web/tm-chateasy-server/removedLogs.txt ~/Desktop/devDump

[azureuser@20.127.14.169](mailto:azureuser@20.127.14.169)