# myled

"myled" is a turn on the led with Linux.

# DEMO

LEDを付けて消しました．<br>
https://youtu.be/VaFWEoOYTV0

# Features

シンプルにLEDをつけたい人向け．

# Requirement

* ubuntu 20.04.3
* Rspberry Pi 4 Model B

# Installation

ubuntu

```bash
sudo apt install gcc
sudo apt install make
```

# tools

Raspberry Pi 4 Model B x 1
LED x 1
抵抗220Ω x 1
オスオスジャンパワイヤ x 2
オスメスジャンパワイヤ x 2
ブレッドボード x 1

# Usage

ディレクトリ内で以下のコマンドを実行．

```bash
git clone https://github.com/hoge/~
cd myled
make
sudo insmod myled.ko
sudo chmod 666 /dev/myled0
echo 1 > /dev/myled0
echo 0 > /dev/myled0
```

# Note

注意点などがあれば書く

# Author

* MinoriKatou
* Chiba Institute of Technology
* s20C1033CR@s.chibakoudai.jp

# License

"myled" is under [GNU General Public License v2.0](https://www.gnu.org/licenses/).

Thank you!
