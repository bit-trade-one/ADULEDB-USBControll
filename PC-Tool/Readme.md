# ファイルリスト

 - USB_LED_Controller
   - USB_LED_Controller.exe　(通常版)
   - USB_LED_Controller_source.zip　(通常版ソースコード)
 - USB_LED_Controller_csv
   - USB_LED_Controller_csv.exe　(CSV制御版)
   - USB_LED_Controller_csv_source.zip　(CSV制御版ソースコード)
 - USB_LED_Controller_multi_csv
   - USB_LED_Controller_multi_csv.exe　(複数台CSV制御版)
   - USB_LED_Controller_multi_csv_source.zip　(複数台CSV制御版ソースコード)
 - LEDCtrlData_sample001.csv　(CSV制御/複数台CSV制御用サンプルCSV)
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
