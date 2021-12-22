# Handyman マクロパッド ビルドガイド（[English](https://github.com/Taro-Hayashi/Handyman/blob/main/README_EN.md)）
- [キット内容](#キット内容)
- [組み立て方（はんだ付けその1）](#組み立て方はんだ付けその1)
- [動作テスト](#動作テスト)
- [組み立て方（はんだ付けその2）](#組み立て方はんだ付けその2)
- [組み立て方（後半）](#組み立て方後半)
- [カスタマイズ](#キーマップの確認変更方法)
- [おまけ](#おまけ)

## キット内容
![](img/IMG_39352.jpg)
||部品名|数| |
|-|-|-|-|
|1|メインボード|1|黒・PCB|
|2|ミドルプレート1|1|透明アクリル・穴の開いている方|
|3|ミドルプレート2|1|透明アクリル|
|4|ボトムプレート|1|黒・PCB|
|5|保護プレート|1|透明アクリル・小さい|
|6|ネジ（短）|9|3mm|
|7|ネジ（中）|3|4mm|
|8|ネジ（長）|12|6mm|
|9|スペーサー（短）|12|3mm メス-メス|
|10|スペーサー（中）|3|4mm メス-オス|
|11|ダイオード|26|1N4148|
|12|リセットスイッチ|1||
|13|ロータリーエンコーダ（水平型）|1|EC11互換品|
|14|ノブ|1||
|15|ロータリーエンコーダ（ホイール）|2|EVQWGD001|
|16|レバースイッチ|1|メインボードに取り付け済み。[取り付け方](lever.md)|
|17|ゴム足|7||

## キット以外に必要なもの
|部品名|数|||
|-|-|-|-|
|Pro Micro コンスルー付き|1||[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/promicro-spring-pinheader)|
|キースイッチ|22|Kailhロープロファイル（V1, V2)||
|キーキャップ|22|対応するもの|すべて1U|
|Micro USB ケーブル|1||

## オプション
|部品名|数|||
|-|-|-|-|
|SK6812MINI-E|22|[取り付け方](led.md)|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/sk6812mini-e-10)|
|WS2812B|6|無くてもバックライトだけ光ります。|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a0800ws-01-10)|
|1N4148W|22|表面実装タイプのダイオード|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a0800di-02-100)|

## 必要な工具
|工具名| |
|-|-|
|はんだごて||
|はんだごて置き場||
|鉛入りはんだ||
|細い+ドライバー|1番ドライバー。|
|細い-ドライバー|先端の幅が2mm以下のもの。|
|ニッパー等ダイオードの足を切れるもの||
|Microsoft Edge、もしくはGoogle Chrome||

## あると便利な工具
|工具名||
|-|-|
|耐熱シリコンマット||
|斜めに切ったタイプのこて先||
|温度調節可能なはんだごて|300度-350度前後。|
|フラックス||
|ピンセット||
|テスター||
|フラックスリムーバー||
|マスキングテープ||
|はんだ吸い取り線||
|はんだ吸い取り器||
|耐熱絶縁テープ（カプトンテープ）||

## 組み立て方（はんだ付けその1）（[画像を反転する](https://github.com/Taro-Hayashi/Handyman/blob/main/README.md#組み立て方はんだ付けその1)）
発送での事故防止のために予め取り付けられている保護プレートとネジ、スペーサーを取り外します。  
![](img/IMG_3936_r.jpg)  
保護プレートは後で使います。ネジ、スペーサーは予備としてお使いください。

はんだ付けのやり方は動画で見るとわかりやすいです。  
パーツは思ったより壊れないので落ち着いて作業すると失敗しにくいです。  
 - ホームセンターのDCMさんの解説動画(58秒～)  [YouTube](https://www.youtube.com/watch?v=JFQg_ObITYE&t=58s)

それではダイオードをD1からD26まで取り付けます。  
足を曲げて裏から差し込みます。  
ダイオードには向きがあります。三角形の先の棒と黒線を合わせましょう。  
![](img/diode1_r.jpg)  

表で更に足を曲げて抜けないようにします。  
ダイオードと並行に曲げるとあとでキースイッチに干渉しにくいです。
![](img/diode2_r.jpg)  

はんだ付けをして足を切ります。  
![](img/diode3_r.jpg)   

リセットスイッチを裏から差し込み表ではんだ付けします。  
![](img/reset1_r.jpg)   
フラックスクリーナーを使う人はここで表面を綺麗にしておきましょう。  
![](img/reset2_r.jpg)   

キースイッチを表から差し込みます。  
![](img/keyswitch1_r.jpg)  
ここの二つのスイッチはPro Microと接触する可能性があるので、足を切ってからはんだ付けします。
![](img/keyswitch2_r.jpg)  
choc V1スイッチの場合、足が一か所干渉するので短くカットしてください。
![](img/keyswitch3_r.jpg)  

メインボードの裏にコンスルーを挿します。  
![](img/promicro1_r.jpg)   
コンスルーの窓が高くて両方とも同じ向きになるように設置します。  
挿すだけではんだ付けはしません。  

コンスルーにPro Microを挿します。TX0, RAW, USBの位置をシルク印刷と合わせましょう。   
USBの端子がショートしやすいのでカプトンテープやマスキングテープをお持ちの方はここで絶縁しておくと安心です。 
![](img/promicro2_5_r.jpg) 
![](img/promicro2_r.jpg)   

Pro Micro側のコンスルーの足を半田付けします。  
![](img/promicro3_r.jpg)   

## 動作テスト
ロータリーエンコーダーを取り付ける前にPro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

下のwebサイトにアクセスしてください。
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware

テストファームウェアを選んでFLASHします。
![](img/remap02.jpg)  
![](img/remap03.jpg)  

キットのリセットスイッチを押すとArduino Microが現れるので、クリックして接続します。
![](img/remap04.jpg) 

書き込みが完了したらウィンドウを閉じて大丈夫です。
![](img/remap05.jpg) 

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。  

## 組み立て方（はんだ付けその1）
SW12、SW14に表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/wheel1.jpg)  

ツメを穴に引っかけてからピンを穴に差し込みます。  
ピンを曲げてしまわないように注意してください。  
![](img/wheel2.jpg)  

差し込めたらはんだ付けします。  
![](img/wheel3.jpg)  

SW20に表から水平型のロータリーエンコーダーを取り付けて裏からはんだ付けします。  
![](img/rot1_r.jpg)  
ピンが曲がらないように気を付けましょう。  
![](img/rot2_r.jpg)  
クリップの部分ははんだ付けしなくても構いません。  
![](img/rot3_r.jpg)  

お疲れ様でした。再び動作を確認して問題がなければはんだ付けは終了です。

## 組み立て方（後半）
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。割れやすいので気をつけましょう。  

![](img/bottom1_r.jpg)  
メインボードの赤丸のネジ穴にスペーサー（中）とスペーサー（短）を止めます。  
画像のようにスイッチがついてる側にスペーサー（中）があるようにしてください。  
![](img/bottom2_r.jpg)  

メインボード裏面の残りのネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/bottom3_r.jpg)  

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/bottom4_r.jpg)  
![](img/bottom5_r.jpg)  

表に保護プレートをネジ（中）で取り付けましょう。
![](img/bottom6_r.jpg)  

キーキャップを取り付けたら先ほどと同様の手順で本番用のファームウェアに更新しましょう。
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware
![](img/remap06.jpg)  

マイナスドライバーでノブを取りつけ、ゴム足を貼ったら完成です。
![](img/nob_r.jpg)  
ノブは直径20mmのものまで取り付けを確認しました。  
![](img/full_r.jpg)  

## キーマップの確認、変更方法
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

JIS配列、MacのUS配列用のキーマップ、普通のキーボードのようなキーマップを用意したのでよろしければ手間を省くのにご利用ください。

## 直角出しサポートプレート（別売）
下端は10度傾いています。  
サポートプレートを使うことで簡単に直角を出すことができます。
机や液タブの端に貼り付けるときに便利です。
![](img/angle_r.png)  
ボトムプレートなしで取り付ける場合は付属のワッシャーでビスの長さを調節してください。

## 9月10日にご購入されたお客さまへ
機能の一部に不具合がございます。  
修正した基板の発送をご案内していますのでご覧ください。  
https://twitter.com/w_vwbw/status/1440305043870154764

## その他
ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/master/keyboards/handyman

VIA用JSONファイル [handyman.json](https://github.com/Taro-Hayashi/Handyman/releases/download/14.19/handyman.json)  

プレートのデザインデータ  
[handyman_plates.zip](https://github.com/Taro-Hayashi/Handyman/releases/download/14.19/handyman_plates.zip)  
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