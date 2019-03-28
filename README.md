# testnet-kore

### Dependencies for KORE v13

```bash
sudo apt-get update
sudo apt-get install -y software-properties-common
sudo add-apt-repository -y ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install -y autotools-dev autoconf automake build-essential bsdmainutils 
sudo apt-get install -y libssl-dev libevent-dev libboost-all-dev libcurl4-openssl-dev 
sudo apt-get install -y libdb4.8-dev libdb4.8++-dev libzmq3-dev 
sudo apt-get install -y libtool pkg-config protobuf-compiler python3 qttools5-dev
sudo apt-get install -y qttools5-dev-tools libprotobuf-dev libqrencode-dev git curl jq

sudo apt-get update && sudo apt-get upgrade -y
```
### To untar package
```bash
tar -zxvf  linux-kore-testnet.tar.gz
```
