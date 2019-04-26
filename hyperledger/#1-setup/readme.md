ref: https://hyperledger.github.io/composer/v0.19/installing/installing-prereqs.html

The following are prerequisites for installing the required development tools:

Operating Systems: Ubuntu Linux 14.04 / 16.04 LTS (both 64-bit)
Docker Engine: Version 17.03 or higher
Docker-Compose: Version 1.8 or higher
Node: 8.9 or higher (note version 9 is not supported)
npm: v5.x
git: 2.9.x or higher

get docker engine from https://get.docker.com/ ($ curl -fsSL https://get.docker.com -o get-docker.sh && sh get-docker.sh)

get node from their repos (curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt-get install -y nodejs) and npm from apt-get

theres a script to check everything is in order :
curl -O https://hyperledger.github.io/composer/v0.19/prereqs-ubuntu.sh

chmod u+x prereqs-ubuntu.sh

you then need to trigger a download of the fabric network (i used hlfv11)
export FABRIC_VERSION=hlfv11
./downloadFabric.sh
./startFabric.sh
./createPeerAdminCard.sh

References:
https://hyperledger.github.io/composer/v0.19/tutorials/deploy-to-fabric-single-org 
https://medium.com/cochain/hyperledger-fabric-on-windows-10-26723116c636