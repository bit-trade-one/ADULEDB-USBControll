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
   
## 複数台制御をするには

複数台制御をするには、それぞれ別のデバイスIDファームウェアが書き込まれたADULEDBと、  
専用の制御ソフトが必要です。  
ファームウェアとは製品に書き込まれたソフトウェアのことを指します。  

下記ファームウェア書き換え手順を実行し、それぞれに別のファームウェアを記載して、  
複数制御ソフトより制御してください。

## ファームウェア書き換え手順

1.基板上のBOOTピンヘッダを、シルク線で結ばれている2本に切り替える
![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/03/DSC_0321.jpg)

2.PCと基板をUSBで接続する

3."USBLEDController_UpdateTool.exe"を起動し、左下が"USB Connected"になっていることを確認する
![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/03/01start.png)

4."Device ID"を1台ずつ変更し、"Update"ボタンをクリックする
![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/03/02select.png)

5."Verification Succesfull"が表示されたらPCから基板を取り外す
![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/03/03update.png)

6.基板上のBOOTピンヘッダを反対側に切り替える
![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/03/DSC_0322.jpg)

上記の手順を設定したい台数分繰り返してください。

## 複数台制御手順

1.[USB_LED_Controller_multi_csv.exe](https://github.com/bit-trade-one/ADULEDB-USBControll/raw/master/PC-Tool/USB_LED_Controller_multi_csv/USB_LED_Controller_multi_csv.exe)をダウンロード・起動する
![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/03/11boot.png)

2.PCと基板をUSBで接続する

3.左下の接続ステータスで接続している制御基板が認識されていることを確認する
![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/03/12connect.png)

4.各基板ごとの\[選択\]ボタンをクリックし、[制御用CSVファイル](https://github.com/bit-trade-one/ADULEDB-USBControll/tree/master/CSV)を開く  
繰り返し制御を行う場合は\[Loop\]のチェックボックスを入れる
![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2022/03/13select.png)

5.ファイルの選択が終わったら\[LED制御開始\]ボタンをクリックする
