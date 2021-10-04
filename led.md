## LEDの取り付け方
LEDのはんだ付けはいつ行っても大丈夫です。  
一旦LEDなしで完成させてから後日やってもいいですし、ファームウェア書き込みの知識がある方は先にLEDだけ付けて発光のテストをすることもできます。  
失敗しても光らないだけなので気軽に挑戦してみてください。   

LEDの切り欠きとシルク印刷のコーナーを合わせてはんだ付けしましょう。  
![](img/led1.jpg)  
![](img/led2.jpg)  
向きがバラバラなので毎回確認してください。  
メインボードにフラックスを塗り、こて先にのせたはんだを流し込むようにするとスムーズに付けられます。  
![](img/led3.jpg)  
両側のランドにはんだを乗せやすいようにLEDは中央に置くことを意識するといいと思います。  

LEDテスト用のファームウェアです。  
- [ledtest_default.tex](https://github.com/Taro-Hayashi/Handyman/releases/download/14.19/ledtest_default.hex)  

LEDは直列に配線されています。  
![](img/led4.jpg)  
ひとつ発光しないLEDがある場合その先のLEDは正しくはんだ付けされていても光らなくなるので画像と見比べてどこが原因かを調べましょう。   

はんだ付けするだけでLEDが使えるようになります。  
ESC長押しでRGB操作用のレイヤーになります。  
![](img/ledlayout.jpg)  
[Keyboard Layout Editor で見る](http://www.keyboard-layout-editor.com/#/gists/b1de3d8b33b46ababd2dff071c8af257)

ブラウザの機能で戻ってください。
