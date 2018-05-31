
NodeMcu-IR-All-in-1
-----------------


<p align="center">
  <img src="img/ESP001.jpg" alt="CH340"/>
</p>




USB燒入晶片驅動程式:

        http://www.wch.cn/download/CH341SER_ZIP.html








需安裝以下工具:

    #include <ESP8266WiFi.h>
    #include <IRremoteESP8266.h>
    #include <IRsend.h>

可選擇以下燒入檔:

    NODEMCU (Arduino IDE)
    NODEMCU (LUA)
    MicroPython

### MicroPython

韌體燒入軟體:

        http://gitlab.trunksys.com:30000/monospace/smart-office/tree/master/%E5%B7%A5%E5%85%B7/nodemcu-flasher-master/nodemcu-flasher-master

可參考:

    http://yhhuang1966.blogspot.tw/2017/04/esp-01-esp8266-micropython.html

### 使用Arduino IDE教學



韌體燒入軟體:

        http://gitlab.trunksys.com:30000/monospace/smart-office/tree/master/%E5%B7%A5%E5%85%B7/nodemcu-flasher-master/nodemcu-flasher-master

請注意板子記憶體下為ESP01 500KB 用的:

        http://gitlab.trunksys.com:30000/monospace/smart-office/blob/master/%E5%B7%A5%E5%85%B7/esp8266-512k-20180207-v1.9.3-278-gcc92c057.bin



ESP01-燒入接線圖
-----------------
<p align="center">
      <img src="img/ESP01A.jpg" alt="CH340"/>
</p>

<p align="center">
      <img src="img/ESP01B.png" alt="CH340"/>
</p>

燒入選項
-------
<p align="center">
      <img src="img/esp8266-micropython.jpg
" alt="CH340"/>
</p>
