# install python2.7.18

sudo apt update && sudo apt upgrade

sudo apt install -y build-essential checkinstall libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev libffi-dev

cd /usr/src

wget https://www.python.org/ftp/python/2.7.18/Python-2.7.18.tgz

tar -xvf Python-2.7.18.tgz

cd Python-2.7.18

./configure --enable-optimizations

make

make install

# Setting Up pip for Python 2.7.18

sudo apt install curl

curl https://bootstrap.pypa.io/pip/2.7/get-pip.py -o get-pip.py

sudo python2.7 get-pip.py

