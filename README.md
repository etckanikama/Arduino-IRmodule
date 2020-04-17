# Arduino-IRmodule
IRセンサを使って自宅にあるリモコンの値を読み取りました

- 赤外線受信センサモジュールの仕様<br>
![Arduino-lesson01](https://user-images.githubusercontent.com/43441878/79557669-e701bd00-80dd-11ea-9048-d004ff520c46.jpg)

G：GND、R：５V、Y：DATA

- 赤外線通信の仕組み<br>
送信側は赤外線LEDの「点灯」、「消灯」を繰り返すことによって命令を送信します。

受信側は、その「点灯」、「消灯」を読み取ることで命令を受信します。

# 概念図
簡単な概念図がこちら。
![Arduino-lesson02](https://user-images.githubusercontent.com/43441878/79557569-bde12c80-80dd-11ea-8af2-dc9cadca8f0f.jpg)

※発光する周波数は、一般的に38[KHz]が使われています。<br>


# 回路図
![Arduino-lesson03](https://user-images.githubusercontent.com/43441878/79557752-0dbff380-80de-11ea-99bb-fa3318e44dc2.jpg)

# コードについて
単純に受信したデータをシリアルモニターに表示するだけのコードです。
＊16進数
００００　⇒　０（１０進数で０）
１１１１　⇒　Ｆ（10進数で１５）
で表示しています。

# 完成図
![iOS の画像 (13)](https://user-images.githubusercontent.com/43441878/79558179-b79f8000-80de-11ea-86f6-0562bfcd7c83.jpg)
