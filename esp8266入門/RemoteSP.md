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
      <img src="/img/smartplug.png" alt="smartplug"/>
</p>


使用函式庫 :

        #include <ESP8266HTTPClient.h>
        #include <ESP8266WiFi.h>
        #include <ArduinoJson.h>
        #include <PubSubClient.h>

記得改ssid :

        
    const char* ssid = "........";
    const char* password = "........";
    char serverAddress[] = "http://############.com";


記得定義腳位 :

        
    #define AC110PIN 4     // Connect ed to Pin D2 in NodeMCU







add code :

    +-  server.on("/on", [](){
          server.send(200, "text/plain", "this works as well");
    ++      digitalWrite(AC110PIN, HIGH);
        });
      

void httpPOST(int value) {
  if (WiFi.status() == WL_CONNECTED) { //Check WiFi connection status

    HTTPClient http;    //Declare object of class HTTPClient

    http.begin("http://############.com/postjson");      //Specify request destination
    http.addHeader("Content-Type", "application/json");  //Specify content-type header

    int httpCode = http.POST(JSONmessageBuffer);   //Send the request
    String payload = http.getString();                                        //Get the response payload
    Serial.print("httpCode:");   //Print HTTP return code
    Serial.println(httpCode);   //Print HTTP return code
    Serial.print("payload:");   //Print HTTP return code
    Serial.println(payload);    //Print request response payload
    /*
      Serial.println(WiFi.macAddress());

    */
    http.end();  //Close connection
  }
  else {
    Serial.println("Error in WiFi connection");
  }
  delay(3000);   //Send a request every 30 seconds
}




https://webduino.io/buy/webduino-developer-smart-socket.html
