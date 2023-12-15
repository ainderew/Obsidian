#### CHATEASY
|   |   |   |   |   |
|---|---|---|---|---|
|TMChatEasyServer0|Azure|[azureuser@20.120.19.74](mailto:azureuser@20.120.19.74)||Kenneth  <br>Andrew|
|TMChatEasyServer1|Azure|[azureuser@13.68.187.112](mailto:azureuser@13.68.187.112)||Kenneth  <br>  <br>Andrew|
|TMChatEasyServer2|Azure|[azureuser@20.127.14.169](mailto:azureuser@20.127.14.169)|
Production
**Server**
ssh -i ~/.ssh/tm-andrew azureuser@20.120.19.74
ssh -i ~/.ssh/tm-andrew azureuser@13.68.187.112
ssh -i ~/.ssh/tm-andrew azureuser@20.127.14.169

**Client**
ssh -i ~/.ssh/tm-andrew azureuser@20.228.229.234

theoria@143.198.77.239

Server SSH Access Checklist

|   |   |   |   |   |
|---|---|---|---|---|
|Server|Platform|User/IP Address/Sudo PW|Sudo Password|Given to|
|dev|DigitalOcean|james@206.189.168.89|theoriamedical|Kenneth  <br>Andy<br><br>Andrew|
|dev2|DigitalOcean|theoria@157.230.55.160|theoriamedical|Kenneth<br><br>Andy  <br>Andrew|
|dev3|DigitalOcean|theoria@143.198.77.239|theoriamedical|Kenneth  <br>Andy<br><br>Andrew|
|staging|DigitalOcean|james@178.128.76.4|theoriamedical|Kenneth<br><br>Andy  <br>Andrew|
|prod-website|DigitalOcean|james@167.71.186.1|5Startelemed|Kenneth  <br>Andy|
|prod-telemed|DigitalOcean|james@157.245.86.93|theoriamedical|Kenneth|
|prod-vpn|DigitalOcean|root@159.89.239.237||Kenneth|
|TMAdminServer0|Azure|james@13.68.196.103||Kenneth|
|TMAdminServer1|Azure|azureuser@40.76.1.234||Kenneth|
|TMAdminServer2|Azure|azureuser@20.120.65.238||Kenneth|
|TMAdminServer3|Azure|azureuser@20.85.229.54||Kenneth|
|TMAdminClient0|Azure|james@13.92.103.11||Kenneth|
|TMAccountsClient0|Azure|james@40.121.91.156||Kenneth|
|TMCharteasyServer0|Azure|azureuser@52.255.190.73||Kenneth|
|TMCharteasyServer1|Azure|azureuser@13.90.91.138||Kenneth|
|TMCharteasyServer2|Azure|azureuser@52.186.73.52||Kenneth|
|TMCharteasyServer3|Azure|azureuser@13.90.115.86||Kenneth|
|TMChearteasyClient0|Azure|azureuser@52.152.136.86||Kenneth|
|TMElasticSearch|Azure|james@13.68.147.137||Kenneth|
|TMRedis|Azure|james@23.96.55.145||Kenneth|
|TMAIAPI|Azure|azureuser@172.174.81.255||Kenneth|
|TMScottishPinesAPI|Azure|azureuser@20.168.212.136||Kenneth|
|PinecrestHL7Listener|Asure|azureuser@52.186.68.19||Kenneth|
|TMIntranetServer0|Azure|james@40.117.121.181||Kenneth  <br>Andy|
|TMIntranetClient|Azure|james@52.249.183.8||Kenneth  <br>Andy|
|TMInstituteServer0|Azure|azureuser@13.82.174.58||Kenneth  <br>Andy|
|TMInstituteClient0|Azure|azureuser@13.82.175.85||Kenneth  <br>Andy|
|TMPrPortalClient0|Azure|azureuser@13.82.190.103||Kenneth  <br>Andy|
|TMChatEasyClient0|Azure|azureuser@20.228.229.234||Kenneth<br><br>Andrew|
|TMChatEasyServer0|Azure|azureuser@20.120.19.74||Kenneth  <br>Andrew|
|TMChatEasyServer1|Azure|azureuser@13.68.187.112||Kenneth<br><br>Andrew|
|TMChatEasyServer2|Azure|azureuser@20.127.14.169||Kenneth<br><br>Andrew|
|TMRabbitMQ0|Azure|azureuser@20.85.219.225||Kenneth  <br>Andrew|
|ChatElectronServer|Azure|azureuser@20.172.157.149||Kenneth  <br>Andrew|

RABBIT_URL=amqp://admin:Tyshs67YhNgahROp9@20.85.219.225:5672
  
  RABBIT_URL=amqp://admin:Tyshs67YhNgahROp9@10.0.1.35:5672

Andy

  

ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQCtIyGKLcsO5HHPF8DF4HnZSifwvfIvu7KcAARqGq6hR/A3dVItMdjm+5/PLavcn30BAc/bFMJbbjCTZ78mRrgBSwDq0ExvViqrZ41T4jgSAcWrB5r3DzpEao2J7wCUEKdqkW/N6UihbCunpDHvTWTJEbCja4MhGWN+jKC0zo8M2Rd9ja+lH6qK6sLi+JIrTqdYYoWBW4jsoHuQkv3pB/YhZINWLPQIyE3qD3CQSiTcBb2tdNlYjh4Cz7XQmGO6wdg+xb1NX/2LbOG4cHnpdgdPR6eVnwFfZweX5mcSxc8vLiv5DnVjanZzPgqbDJa7rbPbd0+V4PsskeFshNInKzxnxdHy2ub6AMOr0+j25lm9T2dQoOASyi7OpvkDNOKXYwKQQbNc1Tw+9MGI+SgdS8JFBufhTYpGXCq1i/dAGitHdABS671SR1OR1L2SgJi9qVewL/hDBYikx2k0GT16inHMrW+ahCUSNes1H4YBM7V2XVb6C1KFy8i52wuW1SV5k2s= peterandrebanua@Peters-MacBook-Pro.local

  

Andrew

  

ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDDmz57jLVswctbGAfVm9xdMoxbEORgolUcRjYZywk4us/AP60LK5FRUI1qQ+WIlmeldxiAPRMYqrUZZxadSPKMleFeelIUxVhh6B6V07rVWt+nfLt4XuSjWxdUyLHlMCL6dast8s7InoaLX6z71pfs88+LINyAchMWla+rruSlFOnsImZCsQNOdl0QRdlidefcBKljh7ssM3iTsqt4aGMDGd7O5awGzGCBesXdginWf1OREzS6Gls5JG9yxFquoxn/WInV0aroAQyHyp78y41tJ78kErBDl1RP0wTSyMM0pdBzJDWVUJc/5GpZWGgwuVa1mONovpBqP6H12GTDzPQtOjU3GwzsdmLyALWGjFTJQiXELKKy5pHxKeDQOii20VlGn4OZRIn1lANn/z/grM2Vb8gpz4Ug5uJ/+prA9gN0xtSgq49KHxfNpZx8454qza7pRVgqjSxBUj2lUMqBbldwaGlYIqABz67A3dOXU3QXOJgvWFtv6kDCe32OAhmKyW8= andrewpinon@Andrews-MacBook-Pro.local

  

Kenneth

  

ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQC6tT7fXpYKKuLKrcRj9YaGP2Yj0DTAMEBFgCcLqbuvydKYiy7c6PoLgaMXieGikILvGho6P1p7hoZ98cUwGB7PBnO0XBvoZ0hUJumyDas3fpK04HqsH5O2loZ2apY+tprN8SAELVFZ3eMaUX8xeI8vm2PnfhPXJK1EAOpQqRTp3QTPCUwmxoM+kEfSyr+nN0siqZlJr9VScNtcMH8faKVdFA+yzaW3Ww3mich9kSC2OH3GxBfqZ3cyniLXmTX267aKVyy9iL47vtZ9HAj2T/yuJnnXufHWnvw/DlOeCRepHmYoePwSWd4dElFM6l/cVopTxYBM1xvx6NDil66HNpPLZvBKF1J6daRZxum8Swi48YYEnb6UZ+7rFs4eq7yjEHUE/OopVeivgOIT2or5xAID2xCTsJVXDfeljMnAHUCE0UMVI7/8+IlzWLWBsD6/9M7Y6C3dHxSEuuv1zvtV82bPukWEcCNyz77E2RJaIHL7py437Cd+aQ0mRm78RWPIgc0= kennmasing@Kenneths-MacBook-Pro.local
