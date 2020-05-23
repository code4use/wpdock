Initialize - create network nginx-proxy and container jwilder/nginx-proxy

./init.sh

mkdir example.com
cd example.com
ln -s ../wp-instance.yml docker-compose.yml
echo VIRTUAL_HOST=example.com > .env
echo LETSENCRYPT_HOST=example.com >> .env
echo LETSENCRYPT_EMAIL=mail@example.com >> .env
docker-compose up -d

