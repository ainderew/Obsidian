
#### Fix for SSH keys not working in MongoDB Compass

<span style="color:red;">Error Message</span>
```` error
"compass" Error creating SSH Tunnel: Error while signing data with privateKey:     error:06000066:public key routines:OPENSSL_internal:DECODE_ERROR
````



SOLUTION: 
Convert the SSH key to the PEM format, which is supported by MongoDB Compass

``` bash
ssh-keygen -p -m PEM -f ~/.ssh/my_private_key
```
