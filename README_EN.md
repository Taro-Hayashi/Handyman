# Handyman マクロパッド Build Manual（[日本語](https://github.com/Taro-Hayashi/Handyman/blob/main/README.md)）
- [Contents](#Contents)
- [Soldering](#Soldering)
- [Testing](#Testing)
- [Assembling](#Assembling)
- [Customise](#Customise)


## Contents
![](img/IMG_39352.jpg)
||Name|Quantities| |
|-|-|-|-|
|1|Main board|1||
|2|Middle plate #1|1||
|3|Middle plate #2|1||
|4|Bottom plate|1||
|5|Cover plate|1||
|6|Short screws|9|3mm|
|7|Middle screws|3|4mm|
|8|Long screws|12|6mm|
|9|Short spacer|12|3mm|
|10|Middle spacer|3|4mm|
|11|Diodes|26|1N4148|
|12|Tactile Switch|1||
|13|Dial rotary encoder|1|EC11|
|14|Knob|1||
|15|Wheel rotary encoder|2|EVQWGD001|
|16|Lever switch|1|Assembled|
|17|Rubber feet|7||

## Additional required
|Name|Quantities||
|-|-|-|
|Pro Micro (With Conthrough)|1|[Yushakobo](https://shop.yushakobo.jp/en/products/promicro-spring-pinheader)|
|Switches|22|Kailh Low Profile Switches V1/V2|
|Keycaps|22|1U|
|Micro-USB Cable|1|[Yushakobo](https://shop.yushakobo.jp/en/products/usb-cable-micro-b-0-8m)|

## Optional
|Name|Quantities||
|-|-|-|
|SK6812MINI-E|22|[Yushakobo](https://shop.yushakobo.jp/en/products/sk6812mini-e-10)|
|WS2812B|6|[Yushakobo](https://shop.yushakobo.jp/en/products/a0800ws-01-10)|

## Soldering
Remove cover plate, screws and spacers.  
![](img/IMG_3936.jpg)  
Cover plate will be used later.  

Install the diodes from D1 to D26.  
![](img/diode1.jpg)  
Diodes have a direction.  

Bend the legs parallel to the diode to prevent interference with the key switch later.  
![](img/diode2.jpg)  

Solder and cut the legs.  
![](img/diode3.jpg)   

Solder Tactile Switches.  
![](img/reset1.jpg)   
If you want to remove the flux from the surface, now is the time.  
![](img/reset2.jpg)   

Solder Switches.  
![](img/keyswitch1.jpg)  
The two switches here may come in contact with the Pro Micro, so cut off the legs before soldering.  
![](img/keyswitch2.jpg)  
In the case of the choc V1 switch, one of the legs will interfere with the switch, so cut it short.  
![](img/keyswitch3.jpg)  

Put conthroughs. Make the top and bottom and front and back the same.  
Conthroughs are not soldered so that Pro Micro can be removed.  
![](img/promicro1.jpg)   

And put Pro Micro on conthroughs.  
![](img/promicro2.jpg)   
If you have Kapton tape or masking tape, you can insulate it here.
![](img/promicro2_5.jpg) 

Solder Pro Micro.  
![](img/promicro3.jpg)   

Solder rotary encoders.  
![](img/wheel1.jpg)  
![](img/wheel2.jpg)  
![](img/wheel3.jpg)  
![](img/rot1.jpg)  
![](img/rot2.jpg)  
![](img/rot3.jpg)  

## Testing
Connect one of them to the PC with a USB cable.  
Access Remap's firmware page with Chrome or Edge.  
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware

Flash the Test firmware.  
![](img/remap02.jpg)  
![](img/remap03.jpg)  

Push the tactile switch.  
![](img/remap04.jpg) 
![](img/remap05.jpg) 

Make sure all switches are responsive.  
If there are no problems, soldering is finished.  

## Assembling
Disconnect the USB cable. 

Attach the short and middle spacers to the red circle.  
![](img/bottom1.jpg)  
There will be middle spacers on the side of the key switch.  
![](img/bottom2.jpg)  

Attach short spacers on the back of the main board with short screws.  
And fit the middle plate #1.  
![](img/bottom3.jpg)  

Fasten the middle plate #2 and the back plate with long screws.  
![](img/bottom4.jpg)  
![](img/bottom5.jpg)  

Attach cover plate to the front with middle screws.  
![](img/bottom6.jpg)  

After installing the keycap, follow the same procedure as before to update the firmware for production.  
- https://remap-keys.app/catalog/dTmFWd6gilf5ziDWE1TR/firmware
![](img/remap06.jpg)  

Attaching the knob and rubber feet.  
![](img/nob.jpg)  
![](img/full.jpg)  

Thank you for your time.  

## Customise
![](img/layout.png)  
[Keyboard Layout Editor](http://www.keyboard-layout-editor.com/#/gists/b1de3d8b33b46ababd2dff071c8af257)  

Access Remap.  
- Remap https://remap-keys.app/

Select the blue button on the left to proceed.  
![](img/remap1.png)  

After Drag-and-Drop the keys, press the flash button in the upper right corner.  
![](img/remap3.png)  

## Misc
Firmware  
https://github.com/Taro-Hayashi/qmk_firmware/tree/master/keyboards/handyman

JSON for Remap/VIA  
[handyman.json](https://github.com/Taro-Hayashi/Handyman/releases/download/14.19/handyman.json)  

Plates data   
[handyman_plates.zip](https://github.com/Taro-Hayashi/Handyman/releases/download/14.31/handyman_plates.zip)  

Used foostan's footprint.  
https://github.com/foostan/kbd/  
https://github.com/foostan/kbd/blob/master/LICENSE  

Used plut0nium's footprint.  
https://github.com/plut0nium/0xLib  
https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

- Yushakobo: https://shop.yushakobo.jp/en/products/2795  
- BOOTH: https://tarohayashi.booth.pm/items/3208122
