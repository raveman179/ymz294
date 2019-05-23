# YMZ294

arduinoでPSG音源を鳴らすための自作拡張基板、PSGshieldについて。



# 各ファイルの詳細

- sample/arduino_YMZ294_lib.zip

  arduinoでYMZ294を使用するためのライブラリー(<https://wp.hrmux.com/?p=973>)

- sample/ymz294test.ino

  testに使用したarduinoスケッチ(<http://curious4dev.mydns.jp/post-362/>)



- arduino_psg_shield.zip

  ガーバーデータ（基板試作メーカーに発注するために必要なファイル）一式

- ymz294_shield.pdf

  PSGshieldの回路図

  

# 概要

秋月電子で購入可能なYAMAHA製PSG音源チップYMZ294を使って、PSG音源ボードを作る。

PSG音源ボードの構成：arduino unoに、今回作成した拡張基板のPSGshieldをスタック。

外部のアンプやスピーカーを使用しなくても単体で完結できる、お手軽仕様を目指した。



ネット上の情報を参考にしながら、フリーの回路設計ソフトkicadにて回路設計を行った。

基板の製造は[fusionPCB](<https://www.fusionpcb.jp/>)に依頼した。

|                             表面                             |                             裏面                             |
| :----------------------------------------------------------: | :----------------------------------------------------------: |
| ![181105_2231~01](https://user-images.githubusercontent.com/22868285/58213503-613e8b80-7d2d-11e9-8dd5-0a0c26153fcc.jpg) | ![181105_2232~01](https://user-images.githubusercontent.com/22868285/58213530-7fa48700-7d2d-11e9-8a84-5f194b57c550.jpg) |

部品を実装するとこのようになる。

![image25](https://user-images.githubusercontent.com/22868285/58214001-2c333880-7d2f-11e9-9a4c-7d2c640ae2ab.jpg)

--------



## 使用した部品について

部品リストは[Akicart](<http://aki.prioris.jp/list/4adb0369-4739-4c3a-ab5e-19493ba98a8a/>)にて作成した。

各部品の詳細についてはリンク先の通販コードから。

「まとめてカートに入れる」から、一括で秋月電子のカートに入れることができる。



## 今後やること、やりたいこと

- PSGshieldとarduinoの間に挟むmidiインターフェースを作る
- 3Dプリンタを使ってケースを作る
- mmlを解釈して当音源ボードで演奏するためのプログラムを作る