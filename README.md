# Handyman マクロパッド ビルドガイド（[English](https://github.com/Taro-Hayashi/Handyman/blob/main/README_EN.md)）
- [キット内容](#キット内容)
- [準備](#準備)
- [はんだ付け](#はんだ付け)
- [動作テスト](#動作テスト)
- [組み立て](#組み立て)
- [カスタマイズ](#カスタマイズ)
- [おまけ](#おまけ)

## キット内容
![](img/IMG_5094.jpg)
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
|18|レバースイッチ|各1|メインボードに取り付け済み。|

### キット以外に必要なもの
|部品名|数||
|-|-|-|
|キースイッチ|22|[Kailh choc V1](https://shop.yushakobo.jp/collections/all-switches/products/pg1350)、もしくは[Kailh Choc V2](https://shop.yushakobo.jp/collections/all-switches/products/kailh-choc-v2)|
|キーキャップ|22|V1は[専用キーキャップ](https://shop.yushakobo.jp/collections/keycaps/For-Choc-v1)、V2は[CherryMX互換](https://shop.yushakobo.jp/collections/keycaps/cherry-mx-%E4%BA%92%E6%8F%9B-%E3%82%AD%E3%83%BC%E3%82%AD%E3%83%A3%E3%83%83%E3%83%97)です。|
|Micro USB ケーブル|1||

### オプション
|部品名|数|||
|-|-|-|-|
|コンスルー 12ピン|2|高さ2.5mm, [使い方](conthrough.md)|[遊舎工房](https://shop.yushakobo.jp/products/31?_pos=1&_sid=ca92edae3&_ss=r&variant=37665714405537) / [TALPKEYBOARD](https://talpkeyboard.net/items/5e056626d790db16e2889233) / [DailyCraftKeyboard](https://shop.dailycraft.jp/products/conthrough)|
|SK6812MINI-E|22|バックライト|[遊舎工房](https://shop.yushakobo.jp/products/sk6812mini-e-10) / [秋月電子通商](https://akizukidenshi.com/catalog/g/gI-15478/)|
|WS2812B|6|アンダーグロー|[遊舎工房](https://shop.yushakobo.jp/products/a0800ws-01-10) / [秋月電子通商](https://akizukidenshi.com/catalog/g/gI-07915/)|
|色違いアクリルプレート（左手用）|||[遊舎工房 - キーボードアクリルプレート](https://shop.yushakobo.jp/collections/services/products/keyboard_acrylic_plate?variant=43890200740071)|
|色違いアクリルプレート（右手用|||[遊舎工房 - キーボードアクリルプレート](https://shop.yushakobo.jp/collections/services/products/keyboard_acrylic_plate?variant=43890207719655)|
|アクリルバックプレート|||[遊舎工房 - キーボードアクリルプレート](https://shop.yushakobo.jp/collections/services/products/keyboard_acrylic_plate?variant=43890215583975)|

### 必要な工具
|工具名|
|-|
|はんだごて|
|こて先クリーナー（こて台）|
|鉛入りはんだ|
|精密ドライバー|
|ニッパー等ダイオードの足を切れるもの|
|マスキングテープ|
|エポシキ接着剤|
|Microsoft Edge、もしくはGoogle Chrome||

### あると便利な工具
|工具名|
|-|
|耐熱シリコンマット|
|温度調節可能なはんだごて|
|斜めに切ったタイプのこて先|
|フラックス|
|フラックスリムーバー、IPA|
|ピンセット|
|耐熱絶縁テープ（カプトンテープ）|
|テスター|
|はんだ吸い取り線|
|はんだ吸い取り器|


## 準備
左右どちらで作るかを選びます。  
![](img/IMG_5091.jpg)  

キットに付属のPro MicroはMicro-USB端子がもげやすいのでエポシキ接着剤で補強します。  
![](img/IMG_4972.jpg)  
両サイドと手前側のはんだ付けされてるところに少し厚めに塗ります。端子の中に入り込まないように気を付けます。
![](img/IMG_5093.jpg)  
コンスルーを使う場合や黒い基板のPro Microを使う場合は必須の工程ではありません。  
乾燥させている間にはんだ付けを進めましょう。  

## はんだ付け
はんだ付けのやり方は動画で見るとわかりやすいです。  
パーツは思ったより壊れないので落ち着いて作業すると失敗しにくいです。  
 - ホームセンターのDCMさんの解説動画(58秒～)  [YouTube](https://www.youtube.com/watch?v=JFQg_ObITYE&t=58s)

### LEDのはんだ付け
LEDを取り付ける場合はメインボードに最初にはんだ付けします。  
 - [LEDの取り付け方](led.md)  

### ダイオード、リセットスイッチのはんだ付け
D1からD26まで取り付けます。  
足を曲げて裏から差し込みます。  
![](img/IMG_5102.jpg)  
ダイオードには向きがあります。三角形の先の棒と黒線を合わせましょう。  

表で更に足を曲げて抜けないようにします。  
![](img/IMG_5103.jpg)  
ダイオードと並行に曲げるとあとでキースイッチに干渉しにくいです。

はんだ付けをして足を切ります。  
![](img/IMG_5104.jpg)   

リセットスイッチを裏から差し込み表ではんだ付けします。  
![](img/IMG_5106.jpg)   
フラックスクリーナーを使う人はここで表面を綺麗にしておきましょう。  
![](img/IMG_5107.jpg)   

### キースイッチのはんだ付け

表から差し込みます。  
![](img/IMG_5108.jpg)  
ここの二つのスイッチはPro Microと接触する可能性があるので、足を切ってからはんだ付けします。　　
![](img/IMG_5109.jpg)  
choc V1スイッチの場合、足が一か所干渉するので短くカットしてください。　　
![](img/IMG_5110.jpg)  
全てのスイッチをはんだ付けします。　　
![](img/IMG_511.jpg)  

### Pro Microのはんだ付け
隠れてしまうダイオードD1の方向が合っているか、キースイッチの足がはんだ付けされているかを再度確認してください。  
Micro-USB端子がショートしやすいのでマスキングテープかカプトンテープで絶縁します。  
![](img/IMG_5113.jpg)  
Pro Microに付属しているピンヘッダの、短い側を基板に差し込みます。  
![](img/IMG_5114.jpg)  

Pro Microを乗せます。TX0, RAW, USBの位置をシルク印刷と合わせましょう。  
![](img/IMG_5115.jpg)  
足をニッパーで切ったらはんだ付けします。  
![](img/IMG_5116.jpg)  
![](img/IMG_5014.jpg)  
基板側もはんだ付けします。  
![](img/IMG_5017.jpg)  

### 動作テスト
ロータリーエンコーダーを取り付ける前にPro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

下のwebサイトにアクセスしてください。
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware

テストファームウェアを選んでFLASHします。
![](img/remap02.jpg)  
![](img/remap03.jpg)  

キット裏面ccのリセットスイッチを押すとArduino Microが現れるので、クリックして接続します。
![](img/remap04.jpg) 

書き込みが完了したらウィンドウを閉じて大丈夫です。
![](img/remap05.jpg) 

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。

Remapを使ってファームウェアの更新ができない場合は、QMK Toolboxをお試しください。
- [QMK Toolboxを使ったファームウェア更新方法](firmware.md)

### ロータリーエンコーダーのはんだ付け
SW12、SW14に表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/IMG_5120.jpg)  

ツメを穴に引っかけてからピンを穴に差し込みます。  
ピンを曲げてしまわないように注意してください。  
![](img/IMG_5121.jpg)  

差し込めたらはんだ付けします。  
![](img/IMG_5122.jpg)  

SW20に表からダイヤル型のロータリーエンコーダーを取り付けて裏からはんだ付けします。  
![](img/IMG_5123.jpg)  
ピンが曲がらないように気を付けましょう。  
![](img/IMG_5124.jpg)  
クリップの部分ははんだ付けしなくても構いません。  
![](img/IMG_5125.jpg)  

お疲れ様でした。再び動作を確認して問題がなければはんだ付けは終了です。

## 組み立て
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。割れやすいので気をつけましょう。  

![](img/IMG_5127.jpg)  
メインボードの赤丸のネジ穴にスペーサー（中）とスペーサー（短）を止めます。  
画像のようにスイッチがついてる側にスペーサー（中）があるようにしてください。  
![](img/IMG_5128.jpg)  

メインボード裏面の残りのネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/IMG_5131.jpg)  

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/IMG_5132.jpg)  
![](img/IMG_5133.jpg)  
ゴム足も貼りました。

表に保護プレートをネジ（中）で取り付けましょう。
![](img/IMG_5134.jpg)  

マイナスドライバーでノブを取りつけ、キーキャップを付けたら完成です。
![](img/IMG_5137.jpg)  

先ほどと同様の手順で本番用のファームウェアに更新しましょう。
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware
![](img/remap06.jpg)  

## カスタマイズ
標準ではUS配列設定でのClip Studio Paintにあわせたキーマップになっています。  
![](img/layout.png)  
[Keyboard Layout Editor で見る](http://www.keyboard-layout-editor.com/#/gists/b1de3d8b33b46ababd2dff071c8af257)  

使わないキーを削除したり使用頻度の高いキーを押しやすい位置に変更してみましょう。  

ChromeかEdgeでRemapにアクセスしてください。  
- Remap https://remap-keys.app/

![](img/remap1.png)  
左を選んで進んでいくとアドレスバーからメッセージが出てキーボードを選択できます。  

ドラッグアンドドロップで変更が終わったら右上のflashボタンを押すと反映されます。  
![](img/remap3.png)  

## 右手用に表示を変える
レイアウトオプションでどちら側か選ぶことができます。  
![](img/h.jpg)  

## レイアウトの保存と復元
⇔アイコンで作ったレイアウトを保存することができます。  
いくつかサンプルがをご用意しました。自分のレイアウトを公開することもできるので是非お試しください。
![](img/re.jpg)  

## その他
ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/tarohayashi/keyboards/tarohayashi/handyman

VIA用JSONファイル [handyman.json](https://github.com/Taro-Hayashi/Handyman/releases/download/14.19/handyman.json)  

プレートのデザインデータ  
[handyman_plates.zip](https://github.com/Taro-Hayashi/Handyman/releases/download/14.35/handyman_plates.zip)  
発注先のルールに沿ってデータを修正してください。  

ご不明な点があればBOOTHのメッセージかtwitterでいつでも聞いてください。   

foostan様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/foostan/kbd/  
https://github.com/foostan/kbd/blob/master/LICENSE  

plut0nium様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/plut0nium/0xLib  
https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />この キット は <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">クリエイティブ・コモンズ 表示 - 継承 4.0 国際 ライセンス</a>の下に提供されています。

- 遊舎工房: https://shop.yushakobo.jp/collections/keyboard/products/2795   
- BOOTH: https://tarohayashi.booth.pm/items/3208122
