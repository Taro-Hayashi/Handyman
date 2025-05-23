# Handyman マクロパッド ビルドガイド（[English](https://github.com/Taro-Hayashi/Handyman/blob/main/README_EN.md)）
- [キット内容](#キット内容)
- [準備](#準備)
- [はんだ付け](#はんだ付け)
- [組み立て](#組み立て)
- [キーのカスタマイズ](#キーのカスタマイズ)
- [その他](#その他)

## キット内容
![](img/IMG_0994.jpg)
||部品名|数| |
|-|-|-|-|
|1|メインボード|各1||
|2|バックプレート|1||
|3|ミドルプレート1|1||
|4|ミドルプレート2|1||
|5|保護プレート|1||
|6|ネジ（短）|9|3mm|
|7|ネジ（中）|3|5mm|
|8|ネジ（長）|12|6mm|
|9|スペーサー（短）|12|3mm|
|10|スペーサー（中）|3|4mm|
|11|ダイオード|26|1N4148|
|12|リセットスイッチ|1||
|13|ロータリーエンコーダ（ダイヤル）|1|EC11互換品|
|14|ノブ|1||
|15|ロータリーエンコーダ（ホイール）|2|EVQWGD001|
|16|ゴム足|7||
|17|Pro Micro|1||

### キット以外に必要なもの
|部品名|数||
|-|-|-|
|キースイッチ|22|[Kailh choc V1](https://shop.yushakobo.jp/collections/all-switches/products/pg1350)、[Kailh Choc V2](https://shop.yushakobo.jp/collections/all-switches/products/kailh-choc-v2)、[Lofree ロープロファイル](https://shop.yushakobo.jp/products/8381)|
|キーキャップ|22|V1は[専用キーキャップ](https://shop.yushakobo.jp/collections/keycaps/For-Choc-v1)、V2,Lofreeは[CherryMX互換](https://shop.yushakobo.jp/collections/keycaps/cherry-mx-%E4%BA%92%E6%8F%9B-%E3%82%AD%E3%83%BC%E3%82%AD%E3%83%A3%E3%83%83%E3%83%97)です。|
|Micro USB ケーブル|1||

### 必要な工具
|工具名|
|-|
|はんだごて|
|はんだ|
|精密ドライバー|
|ニッパー等ダイオードの足を切れるもの|
|マスキングテープ等絶縁できるテープ|
|エポシキ接着剤|

### オプション

LEDを光らせる場合
|部品名|数||
|-|-|-|
|[SK6812MINI-E](https://shop.yushakobo.jp/products/sk6812mini-e-10)|22|バックライト|
|[WS2812B](https://shop.yushakobo.jp/products/a0800ws-01-10)|6|アンダーグロー|

色違いのアクリルプレート
|部品名|数||
|-|-|-|
|[キーボードアクリルプレート（左手用）](https://shop.yushakobo.jp/collections/services/products/keyboard_acrylic_plate?variant=43890200740071)|||
|[キーボードアクリルプレート（右手用）](https://shop.yushakobo.jp/collections/services/products/keyboard_acrylic_plate?variant=43890207719655)|||
|[キーボードアクリルプレート（バックプレート）](https://shop.yushakobo.jp/collections/services/products/keyboard_acrylic_plate?variant=43890215583975)|||

Bluetooth接続について
 - [電池ボックスの使い方](ble.md) 

## 準備
左右どちらで作るかを選びます。  
![](img/IMG_1001.jpg)  

Pro MicroはMicro-USB端子をエポシキ接着剤で補強します。  
![](img/IMG_1011.jpeg)  
両サイドと手前側のはんだ付けされてるところに少し厚めに塗ります。端子の中に入り込まないように気を付けます。
![](img/IMG_1020.jpeg)  
乾燥させている間にはんだ付けを進めましょう。  

## はんだ付け
はんだ付けのやり方は動画で見るとわかりやすいです。  
パーツは思ったより壊れないので落ち着いて作業すると失敗しにくいです。  
 - ホームセンターのDCMさんの解説動画(58秒～)  
[![](http://img.youtube.com/vi/JFQg_ObITYE/0.jpg)](https://www.youtube.com/watch?v=JFQg_ObITYE&t=58s)  

### LEDのはんだ付け（オプション）
LEDを取り付ける場合はメインボードに最初にはんだ付けします。  
 - [LEDの取り付け方](led.md)  

### ダイオード、リセットスイッチのはんだ付け
D1からD26までダイオードを取り付けます。  
足を曲げて裏から差し込みます。  
![](img/IMG_1077.jpeg)  
ダイオードには向きがあります。三角形の先の棒と黒線を合わせましょう。  

表で更に足を曲げて抜けないようにします。  
![](img/IMG_1083.jpeg)  
ダイオードと並行に曲げるとあとでキースイッチに干渉しにくいです。

はんだ付けをして足を切ります。  
![](img/IMG_1086.jpeg)  

リセットスイッチを裏から差し込み表ではんだ付けします。  
![](img/IMG_1096.jpeg)  
フラックスクリーナーを使う人はここで表面を綺麗にしておきましょう。  
![](img/IMG_1102.jpeg)   

### ピンヘッダーのはんだ付け（Pro Microはまだはんだ付けしません）
Pro Microの取り付け場所にピンヘッダーの短い側を差し込みます。
![](img/IMG_1117.jpeg)  
位置決めのためにPro Mioroを乗せますが、はんだ付けはせず表にします。
![](img/IMG_1118.jpeg) 
![](img/IMG_1129.jpeg)  
メインボードにピンヘッダーをはんだ付けします。
![](img/IMG_1134.jpeg)  
Pro Microをいったん外します。

### キースイッチのはんだ付け

ここの二つのキースイッチは足がPro Microと干渉するので短く切ります。
![](img/IMG_1150.jpeg)  
差し込んだ状態で短く切りましょう。
![](img/IMG_1137.jpg)  
Choc V2の場合は3本の足を、Choc V1では2本の足と固定用品の一つを短くします。
![](img/IMG_1145.jpg)  
![](img/IMG_1148.jpg)  
全てのスイッチをはんだ付けします。　　
![](img/IMG_1162.jpeg)  



### Pro Microのはんだ付け
隠れてしまうダイオードD1の方向が合っているか、キースイッチの足がはんだ付けされているかを再度確認してください。  
Micro-USB端子がショートしやすいのでカプトンテープやマスキングテープなどで絶縁します。  
![](img/IMG_1173.jpeg)  
足をニッパーで切ったらはんだ付けします。
![](img/IMG_1174.jpeg)  
![](img/IMG_1184.jpeg)  

### 動作テスト
ロータリーエンコーダーを取り付ける前にPro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

下のwebサイトにアクセスしてください。
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware

テストファームウェアを選んでFLASHします。
![](img/firmwaretest.png)  
![](img/firmware2.png)  

キット裏面のリセットスイッチを押すとArduino Microが現れるので、クリックして接続します（初回のみリセットスイッチを2回押す必要があることがあります）。
![](img/firmware3.png) 

書き込みが完了したらウィンドウを閉じて大丈夫です。

![](img/firmware4.png) 

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。

Remapを使ってファームウェアの更新ができない場合は、QMK Toolboxをお試しください。
- [QMK Toolboxを使ったファームウェア更新方法](firmware.md)

### ロータリーエンコーダーのはんだ付け
SW12、SW14に表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/IMG_1192.jpg)  

ツメを穴に引っかけてからピンを穴に差し込みます。   
![](img/IMG_1200.jpeg)   
ピンを曲げてしまわないように注意してください。  
  
差し込めたらはんだ付けします。  
![](img/IMG_1206.jpeg)  
  
SW20に表からダイヤル型のロータリーエンコーダーを取り付けて裏からはんだ付けします。  
![](img/IMG_1217.jpeg)  
クリップの部分ははんだ付けしなくても構いません。  
![](img/IMG_1223.jpeg)  

お疲れ様でした。再び動作を確認して問題がなければはんだ付けは終了です。

## 組み立て
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。割れやすいので気をつけましょう。  

メインボードのネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/IMG_1299.jpg)   
ここの3箇所は表側はネジではなくスペーサー（中）で止めます。
![](img/IMG_1230.jpg) 

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/IMG_1314.jpeg) 
ゴム足も貼りました。
![](img/IMG_1319.jpeg)  

表に保護プレートをネジ（中）で取り付けましょう。
![](img/IMG_1334.jpeg)  

マイナスドライバーでノブを取りつけ、キーキャップを付けたら完成です。
![](img/IMG_1345.jpeg)  

先ほどと同様の手順でRemap用のファームウェアに更新しましょう。
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware
  
![](img/firmware1.png)  
## キーのカスタマイズ
こちらのサイトにGoogle Chrome（Chromiumベースのブラウザ）でアクセスしてください。
- Remap https://remap-keys.app

![](img/remap1.png)  
左を選んで進んでいくとダイアログが出てキーボードを選択できます。  
![](img/remap2.png)  
選択して接続してください。
![](img/remap3.png)  
標準ではUS配列設定でのClip Studio Paintにあわせたキーマップになっています。  

### キーマップの保存と復元
⇔アイコンで作ったキーマップを保存することができます。  
![](img/remapkey.png)  
作ったキーマップを共有することもできるので是非お試しください。

### 左右を変える
レイアウトオプションで左右を変えることができます。  
![](img/remaplayout.png)  

### キーを設定する
下のキー一覧からドラッグアンドドロップし、変更が終わったら右上のflashボタンを押すと反映されます。  
![](img/remapflash.png)  
また、USキーボードとJISキーボードはFlashの下のプルダウンから変更できます。OSの設定に合わせてください。

### 修飾キーとの組み合わせを設定する
上のキーボードのキーをクリックすると設定画面になります。
![](img/remapmod1.png)  
修飾キーと同時押ししたいキーを検索し、同時押ししたい修飾キーにチェックを入れます。
![](img/remapmod2.png)  

Hold-Tapもここから設定できます。

### ロータリーエンコーダーを設定する
丸いキーの左下をクリックすると時計回り、反時計回り、押し込みを切り替えることができるので、それぞれにキーを割り当てます。
![](img/remapenc.png)  

### 特殊なキーを設定する
FUNCTIONSタブのVIA USER KEYにあらかじめ用意されたショートカットキーがあります。
![](img/remapshortcuts.png)  

### LEDを調整する
このボタンで発光方法を変更することができます。
![](img/remapledset.png)  

## その他

### ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/tarohayashi/keyboards/tarohayashi/handyman

### プレートのデザインデータ  
[handyman_plates.zip](https://github.com/Taro-Hayashi/Handyman/releases/latest/download/handyman_plates.zip)  
発注先のルールに沿ってデータを修正してください。  

### 販売サイト
- 遊舎工房: https://shop.yushakobo.jp/collections/keyboard/products/2795   
- BOOTH: https://tarohayashi.booth.pm/items/3208122
