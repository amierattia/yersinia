
##  Command to Install & Run Yersinia

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install -y gettext autopoint libtool
sudo apt install -y libnet1 libnet1-dev
sudo apt install -y libgtk2.0-dev pkg-config build-essential git autoconf automake

git clone https://github.com/amierattia/yersinia.git
cd yersinia

autoupdate
autoreconf -i
./configure
make
sudo make install

cd src
sudo ./yersinia -G

