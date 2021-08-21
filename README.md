# Handyman マクロパッド ビルドガイド
- [キット内容](#キット内容)
- [組み立て方（はんだ付け）](#組み立て方はんだ付け)
- [動作テスト](#動作テスト)
- [組み立て方（後半）](#組み立て方後半)
- [カスタマイズ](#キーマップの確認変更方法)
- [おまけ](#おまけ)

## キット内容
![パーツ一覧](img/parts.jpg)  
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
|9|スペーサー（短）|12|3mm|
|10|スペーサー（中）|3|4mm|
|11|ダイオード|26|1N4148|
|12|リセットスイッチ|1||
|13|ロータリーエンコーダ（水平型）|1|EC11互換品|
|14|ノブ|1||
|15|ロータリーエンコーダ（ホイール）|2|EVQWGD001|
|16|レバースイッチ|1|SLLB120300, THMU28|
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
|SK6812MINI-E|22|光らせたい場合。[取り付け方](led.md)|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/sk6812mini-e-10)|
|WS2812B|6|無くてもバックライトだけ光ります。|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a0800ws-01-10)|
|1N4148W|22|表面実装タイプのダイオード|[遊舎工房様販売ページ](https://shop.yushakobo.jp/products/a0800di-02-100)|
 
## 必要な工具
|工具名| |
|-|-|
|はんだごて||
|はんだごて置き場||
|鉛入りはんだ||
|フラックス||
|ピンセット||
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
|テスター||
|フラックスリムーバー||
|マスキングテープ||
|はんだ吸い取り線||
|耐熱絶縁テープ（カプトンテープ）||

## 組み立て方（はんだ付け）
はんだ付けのやり方は動画で見るとわかりやすいです。  
パーツは思ったより壊れないので落ち着いて作業すると失敗しにくいです。  
 - ホームセンターのDCMさんの解説動画(58秒～)  [YouTube](https://www.youtube.com/watch?v=JFQg_ObITYE&t=58s)
  
それではダイオードをD1からD26まで取り付けます。  
足を曲げて裏から差し込みます。  
ダイオードには向きがあります。三角形の先の棒と黒線を合わせましょう。  
![](img/diode1.jpg)  
  
表で更に足を曲げて抜けないようにします。  
ダイオードと並行に曲げるとあとでキースイッチに干渉しにくいです。
![](img/diode2.jpg)  
  
はんだ付けをして足を切ります。  
![](img/diode3.jpg)  
  
レバースイッチを取り付けます。  
ランドにフラックスを塗って位置決め用の穴に合わせて乗せます。  
![](img/lever1.jpg)  
  
ピンセットでレバースイッチを押さえながら、はんだごてに乗せたはんだを手前のランドにのせていきます。  
![](img/lever2.jpg)  
  
ちょっとプラスチックを溶かしてしまいましたがこの後ちゃんと動きました。  
![](img/lever3.jpg)  
  
左右はレバーを押さえながらはんだ付けします。  
![](img/lever4.jpg)  
これら4つは取り付け強度を上げるためのランドで、電気的にはどことも繋がっていません。  
  
![](img/lever5.jpg)  
左右にある二股に分かれている接点ははんだが乗りにくいので無理に接着しなくても大丈夫です。  
  
リセットスイッチを裏から差し込み表ではんだ付けします。  
![](img/reset1.jpg)   
フラックスクリーナーを使う人はここで表面を綺麗にしておきましょう。  
![](img/reset2.jpg)   
  
キースイッチを表から差し込みます。  
![](img/keyswitch1.jpg)  
ここの二つのスイッチはPro Microと接触する可能性があるので、足を切ってからはんだ付けします。
![](img/keyswitch2.jpg)  
choc V1スイッチの場合、足が一か所干渉するので短くカットしてください。
![](img/keyswitch3.jpg)  
  
メインボードの裏にコンスルーを挿します。  
![](img/promicro1.jpg)   
コンスルーの窓が高くて両方とも同じ向きになるように設置します。  
挿すだけではんだ付けはしません。  
  
コンスルーにPro Microを挿します。TX0, RAW, USBの位置をシルク印刷と合わせましょう。  
カプトンテープをお持ちの方はここでメインボードとPro Microを絶縁しておくと安心です。  
![](img/promicro2.jpg)   
  
Pro Micro側のコンスルーの足を半田付けします。  
![](img/promicro3.jpg)   
  
SW12、SW14に表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/wheel1.jpg)  
  
ツメを穴に引っかけてからピンを穴に差し込みます。  
ピンを曲げてしまわないように注意してください。  
![](img/wheel2.jpg)  
  
差し込めたらはんだ付けします。  
![](img/wheel3.jpg)  
  
SW20に表から水平型のロータリーエンコーダーを取り付けて裏からはんだ付けします。  
![](img/rot1.jpg)  
ピンが曲がらないように気を付けましょう。  
![](img/rot2.jpg)  
クリップの部分ははんだ付けしなくても構いません。  
![](img/rot3.jpg)  
  
## 動作テスト
Pro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

ファームウェアをダウンロードしてPro Micro Web Updaterにアクセスしてください。
- テスト用ファームウェア [handyman_test.hex](https://github.com/Taro-Hayashi/Shotgun/releases/download/1.0/shotgun_test.hex)
- Pro Micro Web Updater https://sekigon-gonnoc.github.io/promicro-web-updater/index.html

ファイルの選択ボタンを押してダウンロードしたファームウェアを指定したら、flashボタンを押しましょう。  
![](img/promicrowebupdater1.jpg)  

ブラウザのアドレスバーからメッセージが出てきたら、キットのリセットスイッチを押します。      
すると選択欄にArduino Microが出てきてクリックできるようになります。  
![](img/promicrowebupdater2.jpg)  

選択して接続を押すと書き込みが終わります。  
![](img/promicrowebupdater3.jpg)  
ファームウェアを更新する時もこの手順で行います。  

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。
お疲れ様でした。問題がなければはんだ付けは終了です。

## 組み立て方（後半）
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。割れやすいので気をつけましょう。  

![](img/bottom1.jpg)  
メインボードの赤丸のネジ穴にスペーサー（中）とスペーサー（短）を止めます。  
画像のようにスイッチがついてる側にスペーサー（中）があるようにしてください。  
![](img/bottom2.jpg)  
  
メインボード裏面の残りのネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/bottom3.jpg)  

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/bottom4.jpg)  
![](img/bottom5.jpg)  

表に保護プレートをネジ（中）で取り付けましょう。
![](img/bottom6.jpg)  

キーキャップを取り付けたら本番用のファームウェアに更新しましょう。
- [handyman_via.hex](https://github.com/Taro-Hayashi/Shotgun/releases/download/1.0/shotgun_via.hex)

マイナスドライバーでノブを取りつけ、ゴム足を貼ったら完成です。
![](img/nob.jpg)  
ノブは直径20mmのものまで取り付けを確認しました。  
![](img/full.jpg)  

## キーマップの確認、変更方法
標準ではClip Studio Paintにあわせたキーマップになっています。  
![](img/layout.png)  
[Keyboard Layout Editor で見る](http://www.keyboard-layout-editor.com/##@_name=Layout%20-%20Handymman%20MACROPAD%3B&@_y:8.25&t=%23ff29f6&a:7&w:1.25&d:true%3B&=%E8%B5%A4%E6%96%87%E5%AD%97%20%2F=&_x:-0.25&fa@:2%3B&w:2.25&d:true%3B&=%E3%83%87%E3%83%95%E3%82%A9%E3%83%AB%E3%83%88%E8%A8%AD%E5%AE%9A%E3%81%AB%E3%81%AA%E3%81%84%E3%82%B7%E3%83%A7%E3%83%BC%E3%83%88%E3%82%AB%E3%83%83%E3%83%88%3B&@_rx:0.5&x:-0.5&t=%23000000&w:1.25&h:1.25%3B&=Ctrl+S%0A%0A%0A%0A%E4%BF%9D%E5%AD%98&_t=%23ff29f6&w:1.25&h:1.25%3B&=Ctrl+L%0A%0A%0A%0A%EF%BE%84%EF%BD%B0%EF%BE%9D%EF%BD%B6%EF%BD%B0%EF%BE%8C%EF%BE%9E&_t=%23000000&w:1.25&h:1.25%3B&=Shift+%20Ctrl+N%0A%0A%0A%0A%E6%96%B0%E8%A6%8F%E3%83%AC%E3%82%A4%E3%83%A4&_w:1.25&h:1.25%3B&=Ctrl+U%0A%0A%0A%0A%E8%89%B2%E8%AA%BF%E8%A3%9C%E6%AD%A3&_f:1&fa@:3%3B&w:1.25&h:1.25%3B&=Back%20space%3B&@_y:-0.75&x:8.5&f:3%3B&=&=&=&=&_f:1%3B&=%3B&@_y:0.25&x:10.5&c=%23f2c368&fa@:4%3B%3B&=%E6%98%8E%E5%BA%A6+&_x:1&c=%23cccccc%3B&=%3B&@_y:-0.75&x:2&fa@:3%3B&w:1.25&h:1.25%3B&=Ctrl+T%0A%0A%0A%0A%E5%A4%89%E5%BD%A2&_x:1.25&w:1.25&h:1.25%3B&=Ctrl+D%0A%0A%0A%0A%E9%81%B8%E6%8A%9E%E8%A7%A3%E9%99%A4&_x:3.75&c=%23f2c368&fa@:4%3B%3B&=%E5%BD%A9%E5%BA%A6+&_x:1&fa@:3%3B%3B&=%E3%82%B9%E3%83%94%E3%83%BC%E3%83%89+%3B&@_y:-0.75&x:0.75&c=%23cccccc&t=%23ff29f6&w:1.25&h:1.25%3B&=Ctrl+M%0A%0A%0A%0A%EF%BD%B8%EF%BD%B2%EF%BD%AF%EF%BD%B8%EF%BE%8F%EF%BD%BD%EF%BD%B8&_x:1.25&t=%23000000&fa@:4%3B&w:1.25&h:1.25%3B&=M%0A%0A%0A%0A%E9%81%B8%E6%8A%9E%E7%AF%84%E5%9B%B2%3B&@_y:-0.75&x:8.5&c=%23f2c368&f:3&fa@:4%3B%3B&=%E8%89%B2%E7%9B%B8+%3B&@_y:-0.75&x:-0.5&c=%23cccccc&w:1.25&h:1.25%3B&=Shift+F7%0A%0A%0A%0A%E9%81%B8%E6%8A%9E%E3%81%AE%E5%8F%8D%E8%BB%A2&_x:9.75&f:1%3B&=&_x:1%3B&=%3B&@_y:-0.75&x:9.5&c=%23777777%3B&=&_x:1%3B&=&_x:1.5&c=%23cccccc&f:3&w:0.75&h:0.75%3B&=%3B&@_y:-0.75&x:2&f:1&fa@:3%3B&w:1.25&h:1.25%3B&=Ctrl+Z%0A%0A%0A%0A%E3%82%84%E3%82%8A%E7%9B%B4%E3%81%97&_x:1.25&w:1.25&h:1.25%3B&=Ctrl+0%0A%0A%0A%0A%E5%85%A8%E4%BD%93%E8%A1%A8%E7%A4%BA%3B&@_y:-0.75&x:0.75&c=%23777777&w:1.25&h:1.25%3B&=%E3%82%AD%E3%83%A3%E3%83%B3%E3%83%91%E3%82%B9%20%E6%8B%A1%E7%B8%AE&_x:1.25&w:1.25&h:1.25%3B&=%E3%83%96%E3%83%A9%E3%82%B7%E3%82%B5%E3%82%A4%E3%82%BA&_x:1.75&c=%23cccccc&t=%23ff29f6&f:3%3B&=T%0A%0A%0A%0A%E3%83%90%E3%82%B1%E3%83%84&_x:1.25&t=%23000000&f:1%3B&=%3B&@_y:-0.75&x:10.5&c=%23f2c368&fa@:4%3B%3B&=%E6%98%8E%E5%BA%A6%20-&_x:1&c=%23777777&w:0.5&w2:1%3B&=&_x:1&c=%23cccccc&f:3&w:0.75&h:0.75%3B&=%3B&@_y:-0.75&x:-0.5&f:1&fa@:4%3B&w:1.25&h:1.25%3B&=X%0A%0A%0A%0A%E3%82%B5%E3%83%96%E3%82%AB%E3%83%A9%E3%83%BC&_x:8.75&c=%23f2c368%3B&=%E5%BD%A9%E5%BA%A6%20-&_x:1&fa@:3%3B%3B&=%E3%82%B9%E3%83%94%E3%83%BC%E3%83%89-%3B&@_y:-0.5&x:2&c=%23cccccc&w:1.25&h:1.25%3B&=Y%0A%0A%0A%0A%E7%B7%9A%E4%BF%AE%E6%AD%A3&_x:1.25&c=%23777777&w:1.25&h:1.25%3B&=%E3%82%AD%E3%83%A3%E3%83%B3%E3%83%91%E3%82%B9%20%E5%9B%9E%E8%BB%A2&_x:0.5&c=%23cccccc&f:3%3B&=&_x:1.25&c=%23f2c368&f:1&fa@:4%3B%3B&=%E8%89%B2%E7%9B%B8%20-%3B&@_y:-0.75&x:0.75&c=%23cccccc&t=%23ff29f6&fa@:3%3B&w:1.25&h:1.25%3B&=S%0A%0A%0A%0A%E5%AE%9A%E8%A6%8F&_x:1.25&t=%23000000&fa@:4%3B&w:1.25&h:1.25%3B&=I%0A%0A%0A%0A%E3%82%B9%E3%83%9D%E3%82%A4%E3%83%88&_x:9.5&f:3&w:0.75&h:0.75%3B&=%3B&@_y:-0.75&x:9.5&c=%23f2c368%3B&=%3B&@_y:-0.75&x:-0.5&c=%23cccccc&f:1&fa@:4%3B&w:1.25&h:1.25%3B&=O%0A%0A%0A%0A%EF%BD%B5%EF%BE%8C%EF%BE%9E%EF%BD%BC%EF%BE%9E%EF%BD%AA%EF%BD%B8%EF%BE%84%3B&@_y:-0.75&x:8.5&f:2%3B&=%3B&@_y:-0.75&x:6.25&f:3%3B&=G%0A%0A%0A%0A%E3%82%B0%E3%83%A9%E3%83%87&_x:6.75&f:1&w:0.75&h:0.75%3B&=%3B&@_y:-0.75&x:0.75&t=%23000000%0A%239c762f&a:5&f:2&fa@:4&:3%3B&w:1.25&h:1.25%3B&=U%0A%E9%95%B7%E6%8A%BC%E3%81%97LED%0A%0A%0A%E5%9B%B3%E5%BD%A2%3B&@_y:-0.5&x:-0.5&t=%23ff29f6&a:7&f:3&w:1.25&h:1.25%3B&=Ctrl+H%0A%0A%0A%0A%E5%B7%A6%E5%8F%B3%E5%8F%8D%E8%BB%A2&_x:13.25&t=%23000000&w:0.75&h:0.75%3B&=%3B&@_y:-0.5&x:6.25&f:1%3B&=%3B&@_x:6.25&f:3%3B&=J%0A%0A%0A%0A%E8%89%B2%E6%B7%B7%E3%81%9C%3B&@_r:15&rx:1.25&y:1.5&x:13&c=%23f2c368&f:1&fa@:2%3B%3B&=%E6%AC%A1%E3%81%AE%E3%83%91%E3%82%BF%E3%83%BC%E3%83%B3%3B&@_y:2&x:5.5&c=%23aaaaaa&t=%23000000%0A%232a49b5&a:5&fa@:4&:3%3B&w:1.25&h:1.25%3B&=P%0A%E9%95%B7%E6%8A%BC%E3%81%97Shift%0A%0A%0A%E3%83%9A%E3%83%B3%3B&@_r:-30&rx:1.5&ry:2.5&y:7.75&x:6.25&c=%23f2c368&t=%23000000&a:7&fa@:2%3B%3B&=%E5%89%8D%E3%81%AE%E3%83%91%E3%82%BF%E3%83%BC%E3%83%B3%3B&@_ry:3&y:4&x:-1.5&c=%23aaaaaa&t=%23000000%0A%232a49b5&a:5&fa@:5&:3%3B&w:1.25&h:1.25%3B&=E%0A%E9%95%B7%E6%8A%BC%E3%81%97%20Alt%0A%0A%0A%E6%B6%88%E3%81%97%E3%82%B4%E3%83%A0%3B&@_r:-15&rx:0.25&ry:0.5&y:6.5&x:1.75&t=%0A%232a49b5&f:2&fa@:4&:3%3B&w:1.25&h:1.25%3B&=B%0A%E9%95%B7%E6%8A%BC%E3%81%97%20Ctrl%0A%0A%0A%E3%83%96%E3%83%A9%E3%82%B7%3B&@_x:10&c=%23f2c368&t=%23000000&a:7%3B&=ON%2F%2FOFF)  

使わないキーを削除したり使用頻度の高いキーを押しやすい位置に変更してみましょう。  
  
ChromeかEdgeでRemapにアクセスしてください。  
- Remap https://remap-keys.app/
  
![](img/remap1.png)  
左を選んで進んでいくとアドレスバーからメッセージが出てキーボードを選択できます。  
  
ドラッグアンドドロップで変更が終わったら右上のflashボタンを押すと反映されます。  
![](img/remap3.png)  
  
## その他
ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/master/keyboards/handyman
  
VIA用JSONファイル [handyman.json]()  
  
プレートのデザインデータ  
[handyman_plates.zip]()  
発注先のルールに沿ってデータを修正してください。  

ご不明な点があればBOOTHのメッセージやtwitterでいつでも聞いてください。  
販売ページ: https://tarohayashi.booth.pm/items/3172502
  
foostan様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/foostan/kbd/  
https://github.com/foostan/kbd/blob/master/LICENSE  
  
plut0nium様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/plut0nium/0xLib  
https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  
  
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />この キット は <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">クリエイティブ・コモンズ 表示 - 継承 4.0 国際 ライセンス</a>の下に提供されています。
