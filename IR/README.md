[![Build Status](https://travis-ci.org//monospaceIOT//monospaceIOT.png?branch=master)](https://travis-ci.org//monospaceIOT//monospaceIOT) [![Coverage Status](https://coveralls.io/repos//monospaceIOT//monospaceIOT/badge.png?branch=master)](https://coveralls.io/r//monospaceIOT//monospaceIOT?branch=master)

The Workshop project
=======================

```
  __  __                                             /$$$$$$  /$$$$$$  /$$$$$$$$
 |  \/  |                                           |_  $$_/ /$$__  $$|__  $$__/
 | \  / | ___  _ __   ___  ___ _ __   __ _  ___ ___   | $$  | $$  \ $$   | $$   
 | |\/| |/ _ \| '_ \ / _ \/ __| '_ \ / _` |/ __/ _ \  | $$  | $$  \ $$   | $$   
 | |  | | (_) | | | | (_) \__ \ |_) | (_| | (_|  __/  | $$  | $$  \ $$   | $$   
 |_|  |_|\___/|_| |_|\___/|___/ .__/ \__,_|\___\___|  | $$  | $$  \ $$   | $$   
                              | |                    /$$$$$$|  $$$$$$/   | $$
                              |_|                   |______/ \______/    |__/  

```

## [採購請單與規劃請按此](/規劃&採購清單/採購清單&規劃.md).



`WARNING`: 在操作本專案任何項目時請保持`清醒`、`不要短路`、`專注`、`環境安全`、`不要用沒有USB埠電源防護的電腦`.

基本環境安裝
----------------


Arduino IDE :

    https://www.arduino.cc/

圖形化的Arduino IDE (S4A):

    http://s4a.cat/

Arduino 安裝說明 (DL):

<p align="center">
  <img src="/img/ArduinoDL.gif" alt="Arduino DL"/>
</p>

Arduino 安裝說明 (Setup):

<p align="center">
  <img src="/img/ArduinoSetup.gif" alt="Arduino DL"/>
</p>

如果你用的是LINUX:


[Arduino LINUX](https://downloads.arduino.cc/arduino-1.8.4-linux64.tar.xz)




如果你用的是MAC:

[Arduino OF mac ](https://downloads.arduino.cc/arduino-1.8.4-macosx.zip)



========================================================================
"ESP8266" or "NodeMcu" 基本環境安裝
----------------



  安裝說明 (DL):

<p align="center">
  <img src="/img/ESPSetup.gif" alt="Arduino DL"/>
</p>

文字說明:

        $ .//monospaceIOT
        >>> list(5 * x + y for x in range(10) for y in [4, 2, 1])






電路圖接線
----------------

個單元電路圖使用Fritzing繪製，請進入個單元目錄閱讀說明文件.


 Fritzing:

<p align="center">
  <img src="/img/Fritzing.PNG" alt="Fritzing"/>
</p>




# 開發板

Arduino
-----------------

<p align="center">
  <img src="/img/arduino-uno.png" alt="Arduino NUO"/>
</p>



ESP8266-01
-----------------

<p align="center">
  <img src="/img/ESP001.jpg" alt="ESP8266-01"/>
</p>


### 使用Arduino IDE教學


  韌體燒入器:
<p align="center">
    <img src="/img/ESP01A.jpg" alt="CH340"/>
    <img src="/img/ESP01B.png" alt="CH340"/>
</p>


韌體燒入軟體:

        http://gitlab.trunksys.com:30000/monospace/smart-office/tree/master/%E5%B7%A5%E5%85%B7/nodemcu-flasher-master/nodemcu-flasher-master

請注意板子記憶體下為ESP01 500KB 用的:

        http://gitlab.trunksys.com:30000/monospace/smart-office/blob/master/%E5%B7%A5%E5%85%B7/esp8266-512k-20180207-v1.9.3-278-gcc92c057.bin


NodeMcu-CH340
-----------------

<p align="center">
  <img src="/img/ESP8266CH340.jpg" alt="CH340"/>
</p>

USB晶片驅動程式:

        http://www.wch.cn/download/CH341SER_ZIP.html


NodeMcu-CP2102
-----------------

<p align="center">
  <img src="/img/nodemcu-CP2102.png" alt="CP2102"/>
</p>
USB晶片驅動程式:

        https://www.silabs.com/products/development-tools/software/usb-to-uart-bridge-vcp-drivers



韌體燒入器:

        http://gitlab.trunksys.com:30000/monospace/smart-office/tree/master/%E5%B7%A5%E5%85%B7/nodemcu-flasher-master/nodemcu-flasher-master

請注意板子記憶體下為NodeMcu通用的:

        http://
