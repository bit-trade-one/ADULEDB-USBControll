# ファイルリスト

 - ID.zip
   -  FW_LEDController_id*.hex  
      デバイスID別ファームウェア
 - FW_LEDController_v100.zip  
   ファームウェア
 - FW_LEDController_v100_source.zip  
   ファームウェアソース  
 - USBLEDController_UpdateTool.exe  
   ファームウェア書き換えツール

## ファームウェア書き換え手順

1.基板上のBOOTピンヘッダを、シルク線で結ばれている2本に切り替える

2.PCと基板をUSBで接続する

3."USBLEDController_UpdateTool.exe"を起動する

4.左下が"USB Connected"になっていることを確認する

5."Device ID"を1台ずつ変更し、"Update"ボタンをクリックする

6."Verification Succesfull"が表示されたらPCから基板を取り外す

7.基板上のBOOTピンヘッダを反対側に切り替える

上記の手順を設定したい台数分繰り返してください。

## 複数台制御手順

1.[USB_LED_Controller_multi_csv.exe](https://github.com/bit-trade-one/ADULEDB-USBControll/raw/master/PC-Tool/USB_LED_Controller_multi_csv/USB_LED_Controller_multi_csv.exe)を起動する

2.PCと基板をUSBで接続する

3.左下の接続ステータスで接続している制御基板が認識されていることを確認する

4.各基板ごとの\[選択\]ボタンをクリックし、[制御用CSVファイル](https://github.com/bit-trade-one/ADULEDB-USBControll/tree/master/PC-Tool)を開く

5.繰り返し制御を行う場合は\[Loop\]のチェックボックスを入れる

6.ファイルの選択が終わったら\[LED制御開始\]ボタンをクリックする
