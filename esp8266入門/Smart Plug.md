[![Build Status](https://travis-ci.org//monospaceIOT//monospaceIOT.png?branch=master)](https://travis-ci.org//monospaceIOT//monospaceIOT) [![Coverage Status](https://coveralls.io/repos//monospaceIOT//monospaceIOT/badge.png?branch=master)](https://coveralls.io/r//monospaceIOT//monospaceIOT?branch=master)

The Workshop project
=======================

```


 __          __        _        _                 
 \ \        / /       | |      | |                
  \ \  /\  / /__  _ __| | _____| |__   ___  _ __  
   \ \/  \/ / _ \| '__| |/ / __| '_ \ / _ \| '_ \
    \  /\  / (_) | |  |   <\__ \ | | | (_) | |_) |
     \/  \/ \___/|_|  |_|\_\___/_| |_|\___/| .__/
                                           | |    
                                           |_|    


```




`WARNING`: 在操作本專案任何項目時請保持`清醒`、`不要短路`、`專注`、`環境安全`、`不要用沒有USB埠電源防護的電腦`.



========================================================================







# 開發板

Arduino
-----------------

<p align="center">
  <img src="/img/arduino-uno.png" alt="Arduino NUO"/>
</p>



NodeMcu-CH340
-----------------

<p align="center">
  <img src="/img/ESP8266CH340.jpg" alt="CH340"/>
</p>



電路圖接線
----------------

個單元電路圖使用Fritzing繪製，請進入個單元目錄閱讀說明文件.


 Fritzing:

<p align="center">
  <img src="/img/Fritzing.PNG" alt="Fritzing"/>
</p>


nodeMCU接線圖
-----------------
<p align="center">
      <img src="img/smartplug.png" alt="CH340"/>
</p>


使用函式庫 :

        #include <ESP8266WiFi.h>
        #include <WiFiClient.h>
        #include <ESP8266WebServer.h>
        #include <ESP8266mDNS.h>

記得改ssid :

        
    const char* ssid = "........";
    const char* password = "........";

記得定義腳位 :

        
    #define AC110PIN 4     // Connect ed to Pin D2 in NodeMCU





add code :

        http://gitlab.trunksys.com:30000/monospace/smart-office/tree/master/%E5%B7%A5%E5%85%B7/nodemcu-flasher-master/nodemcu-flasher-master


add code :

    +-  server.on("/on", [](){
          server.send(200, "text/plain", "this works as well");
    ++      digitalWrite(AC110PIN, HIGH);
        });
      



