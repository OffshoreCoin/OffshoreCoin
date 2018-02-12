
Working update for Offshore Coin [OFFSHORE]

O/S: Ubuntu 12.04
Name: OFFSHORECOIN
Symbol: OFFSHORE
Algorithm: SHA256,POW
Block Reward: 22 Block
Reward Halving Rate: 14400
Block time: 240 sec
Difficulty retarget: Dark Gravity Wave 
Total supply: 6,553,600 

RPC port: 8015
Net port: 8016


Trading: https://yobit.net/en/trade/OFFSHORE/BTC

To compile: 

sudo apt-get update

sudo apt-get install -y git make g++ build-essential libminiupnpc-dev

sudo apt-get install -y libdb++-dev libssl-dev libboost1.48-all libboost-chrono1.48-dev

git clone https://github.com/Offshore-Coin/OffshoreCoin.git 

cd OffshoreCoin/src/leveldb

chmod +x build_detect_platform 

cd ../..

To compile daemon only:
cd src/
make -f makefile.unix

To compile qt wallet
sudo apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler

qmake offshorecoin-qt.pro

Update 19 Jan 2018
make
