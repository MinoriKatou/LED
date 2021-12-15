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

# tools

Raspberry Pi 4 Model B x 1<br>

LED x 1<br>

抵抗330Ω x 1<br>

オスオスジャンパワイヤ x 2<br>

オスメスジャンパワイヤ x 2<br>

ブレッドボード x 1<br>

# Circuit Diagram

![image](https://user-images.githubusercontent.com/93694457/146138311-514a2cd9-35ab-4d2d-aa58-5b760f3f3c59.png)


![S__26312731](https://user-images.githubusercontent.com/93694457/146136522-9e81728b-2aa8-4c44-a57d-1fdd5d6341b5.jpg)

# Usage

ディレクトリ内で以下のコマンドを実行．

```bash
git clone https://github.com/hoge/~
cd myled
make
sudo insmod myled.ko
sudo chmod 666 /dev/myled0
```
以下コマンドで点灯

```bash
echo 1 > /dev/myled0
```

以下コマンドで消灯

```bash
echo 0 > /dev/myled0
```

実行後のディレクトリの後処理は以下コマンド

```bash
make clean
```

# Note

* GPIO25ピンを利用した回路です．
* LEDは向きがあるので気を付けて．

# Author

* MinoriKatou
* Chiba Institute of Technology
* s20C1033CR@s.chibakoudai.jp

# License

"myled" is under [GNU General Public License v2.0](https://www.gnu.org/licenses/).

Thank you!
