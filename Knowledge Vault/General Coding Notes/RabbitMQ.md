Start RabbitMQ local
```bash
sudo rabbitmq-server
```

Check queues
```bash
sudo rabbitmqctl list_queues
```

Check rabbitMQ statuses
```bash
sudo rabbitmqctl status
```

Changing rabbitmq.conf
```bash
sudo vim /etc/rabbitmq/rabbitmq.conf
```

When changing rabbitmq.conf
	turn it off and on restarting won't work
```bash
sudo systemctl stop rabbitmq-server
sudo systemctl start rabbitmq-server
```


Setting TTL 
	- 600000 is in ms, equals to 60 seconds.
```bash
sudo rabbitmqctl set_policy TTL ".*" '{"message-ttl":3600000}' --apply-to queues
```

Setting Queue Expiry
```bash
sudo rabbitmqctl set_policy expiry ".*" '{"expires":1800000}' --apply-to queues|
```

Access the local in your local machine
```bash
ssh -i ~/.ssh/tm-andrew -L 15672:localhost:15672 azureuser@20.85.219.225
```
It's the -L


curl -i -u guest: guest http://localhost:15672/api/queues/%2f/amq.gen-1-vUYTg0p-OKxyESCrMJ5w/get

curl -i -u guest:guest http://20.85.219.225:15672/api/queues/%2f/amq.gen-1-vUYTg0p-OKxyESCrMJ5w/get