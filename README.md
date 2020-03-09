# buildbottest-cfg
Experiments with Buildbot

buildbot has general documentation here http://docs.buildbot.net/current/index.html

To get buildbot docker compose recipe going on AWS Lightsail (OS Only, Ubuntu 18.04 LTS)

## as root
```
sudo bash
```

```
apt-get update
apt-get upgrade
apt-get install docker-compose
apt install python-twisted-core
usermod -G docker ubuntu
```

## as ubuntu
```
mkdir clima-buildbot
cd clima-buildbot 
git clone  https://github.com/buildbot/buildbot-docker-example-config 
cd buildbot-docker-example-config/simple
docker-compose up
```

## from local system
ssh -i MYKEY.pem -L 8010:localhost:8010 -l ubuntu LIGHTSAILVMIP

