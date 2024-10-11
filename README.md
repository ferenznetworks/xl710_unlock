# xl710_unlock

Este programa desbloqueia NICs Intel xl710.
##
This program unlocks intel xl710 NICs.

## Modo de usar
## Usage

```shell
# ./xl710_unlock -n enp4s0f0
EMP SR offset: 0x67a8
PHY offset: 0x68f6
PHY data struct size: 0x000c
MISC: 0x6b0c <- locked
MISC: 0x6b0c <- locked
MISC: 0x6b0c <- locked
MISC: 0x6b0c <- locked
Ready to fix it? [y/N]: y
```
## Exemplo em um Debian 12
## Example on a Debian 12

```shell
apt update -y && apt upgrade -y
apt install wget zip unzip make gcc -y
wget https://github.com/ferenznetworks/xl710_unlock/archive/refs/heads/main.zip
unzip master.zip
cd xl710_unlock-master
make
./xl710_unlock -n NOMEDAINTERFACE-EX-ENO1
```
