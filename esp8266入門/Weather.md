# 簡易氣象站



--------------------
- 使用作業系統：raspbian
[raspbian-下載](https://www.raspberrypi.org/downloads/raspbian/)




簡易氣象站長這樣
-----------------
<p align="center">
  <img src="img/LIRC/lircRPI.jpg" alt="12VRI"/>
</p>


接線圖
-----------------
<p align="center">
  <img src="img/LIRC/irlc.png" alt="12VRI"/>
</p>



腳位:

    DHT11/22<------> gpio_in_pin=18
    IR接收模組<------> gpio_out_pin=17
    土壤濕度模組<------>
    DHT11/22溫度模組<------>
    DS20水溫模組<------>




需準備以下零件:

    土壤濕度模組
    DHT11/22溫度模組
    DS20水溫模組
    *或是可以買現成的*

說明:

        將RI訊號錄製為 RAW 訊號
        藉由GPIO即可對IR電路送出波形
        由於訊號強度(電壓)不足所以距離很短


進階範例:

        GITHUB
        環境控制系統
