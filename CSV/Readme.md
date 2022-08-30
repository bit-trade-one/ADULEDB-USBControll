# filelist
[ダウンロード](https://github.com/bit-trade-one/ADULEDB-USBControll/raw/master/CSV/LEDCtrlData_sample.zip)・展開してお使いください。  

- LEDCtrlData_sample.zip(CSV制御/複数台CSV制御用サンプルCSV)
  - LEDCtrlData_sample001.csv　
  - LEDCtrlData_sample002.csv
  - LEDCtrlData_sample003.csv
  - LEDCtrlData_sample004.csv

# LED制御CSV仕様

1行ごとに制御開始からの経過秒数でLEDの輝度を指定します。

time\[s\],LED1,LED2,LED3,LED4,LED5,LED6,LED7,LED8,LED9,LED10

 - time:制御開始からの経過秒数 0.01秒単位で記入
 - LEDn:各LEDの輝度(nは1\~10) 0\~100まで1単位で記入

例:
```
0,  0,  0,  0,  0,  0,  0,  0,  0,  0,  0
1, 10,  0,  0,  0,  0,  0,  0,  0,  0,  0
3,  0, 30,  0,  0,  0,  0,  0,  0,  0,  0
5,  0,  0, 50,  0,  0,  0,  0,  0,  0,  0
…
```
上記のcsvで
 - 起動時全消灯
 - 1秒経過で1番LEDが10％、他は消灯
 - 3秒経過で3番LEDが30％、他は消灯
 - 5秒経過で5番LEDが50％、他は消灯

となります。
