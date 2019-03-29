# testnet-kore

### Installation Steps

Note1: that you can speed up the compilation using the option -j when using make, for example: make -j3

Note2: If you machine has less than 3G memory, you should use a swapfile.

a) enabling swap

```bash
    sudo dd if=/dev/zero of=/swapfile bs,=4096 count=1048576
    sudo chmod 600 /swapfile
    sudo mkswap /swapfile
    sudo swapon /swapfile
```

b) disabling swap

```bash
    sudo swapoff -v /swapfile
    sudo rm /swapfile
```

### Installating dependencies

```bash
sudo apt-get update
sudo apt-get install -y software-properties-common
sudo add-apt-repository -y ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install -y autotools-dev autoconf automake build-essential bsdmainutils 
sudo apt-get install -y libssl-dev libevent-dev libboost-all-dev libcurl4-openssl-dev sudo apt-get install -y libdb4.8-dev libdb4.8++-dev libzmq3-dev 
sudo apt-get install -y libtool pkg-config protobuf-compiler python3 qttools5-dev
sudo apt-get install -y qttools5-dev-tools libprotobuf-dev libqrencode-dev git curl jq

sudo apt-get update && sudo apt-get upgrade -y
```

### Building KORE dependencies

```bash
cd depends
make
```

### Building KORE source

```bash
cd ..
./autogen.sh
./configure --with-gui=qt5 --prefix=$(pwd)/depends/x86_64-pc-linux-gnu

make
```

### Testnet Onion Address

```bash
Here are some testnet onion address.
you can use the console from kore-qt and give the command to add
addnode a3y4tqttfcj7dvf3.onion onetry
addnode mnzwvlk7lme5yuht.onion onetry
```

### To untar package
```bash
tar -zxvf  linux-kore-testnet.tar.gz
```
