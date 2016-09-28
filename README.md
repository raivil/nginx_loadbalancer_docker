# Simple Nginx loadbalancer using Docker containers.
Example Nginx LoadBalancer using Docker containers.


### Generate a simple certificate
```sh
openssl genrsa -out domain.com.key 4096
openssl req -new -key domain.com.key -out domain.com.csr
openssl x509 -req -days 365 -in domain.com.csr -signkey domain.com.key -out domain.com.crt
cat domain.com.crt domain.com.key | tee domain.com.pem
```
