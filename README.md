# WireGuard Server Docker


## Installing Docker
- ```sudo apt update```
- ```sudo apt install apt-transport-https ca-certificates curl software-properties-common```
- ```curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -```
- ```sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"```
- ```apt-cache policy docker-ce```
- ```sudo apt install docker-ce```
- ```sudo systemctl status docker```
- ```docker run hello-world```
- ```docker system prune -a```

## Installing GIT and clone repo
- ```sudo apt install git```
- ```mkdir wireguard```
- ```cd wireguard```
- ```git clone https://github.com/guitaristdave/vpn.git```

>[!IMPORTANT]
>## Change the number of users
>In docker-compose.yml file edit the PEERS value (default PEERS=1)

## Up Docker container
- ```docker-compose up -d```
