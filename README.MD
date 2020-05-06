Initialize - create network nginx-proxy and container jwilder/nginx-proxy

./init.sh

mkdir example.com
cd example.com
ln -s ../wp-instance.yml docker-compose.yml
VIRTUAL_HOST=example.com docker-compose up -d

