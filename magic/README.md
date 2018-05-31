[![Build Status](https://travis-ci.org//monospaceIOT//monospaceIOT.png?branch=master)](https://travis-ci.org//monospaceIOT//monospaceIOT) [![Coverage Status](https://coveralls.io/repos//monospaceIOT//monospaceIOT/badge.png?branch=master)](https://coveralls.io/r//monospaceIOT//monospaceIOT?branch=master)

智慧鏡 project
=======================

```

__  __             _                  _                     
|  \/  | __ _  __ _(_) ___   _ __ ___ (_)_ __ _ __ ___  _ __
| |\/| |/ _` |/ _` | |/ __| | '_ ` _ \| | '__| '__/ _ \| '__|
| |  | | (_| | (_| | | (__  | | | | | | | |  | | | (_) | |   
|_|  |_|\__,_|\__, |_|\___| |_| |_| |_|_|_|  |_|  \___/|_|   
             |___/                                          
```




`WARNING`: 在操作本專案任何項目時請保持`清醒`、`不要短路`、`專注`、`環境安全`、`不要用沒有USB埠電源防護的電腦`.

基本環境安裝
----------------

準備材料:

        樹梅派2+無線網卡
        或
        樹梅派3

        HDMI螢幕與差不多小的單向鏡
        (雙面鏡或高反射半反射全反射玻璃)

        外接觸控板(選用)
        外部感測器(選用)

安裝方法:

- 使用作業系統：raspbian
[raspbian-下載](https://www.raspberrypi.org/downloads/raspbian/)

- 將樹梅派的記憶卡插入電腦

- 找到檔案 /boot/config.txt

- 加入以下文字 (設定 顯示器):

            dtoverlay=lirc-rpi,gpio_in_pin=18,gpio_out_pin=17

- 安裝 Magic mirror:

            https://github.com/MichMich/MagicMirror


  安裝說明 (待補GIF):

<p align="center">
  <img src="/img/ESPSetup.gif" alt="待補GIF DL"/>
</p>

文字說明:

        待補
