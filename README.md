#### [GitHubの使い方はこちらの記事をご確認ください。](https://bit-trade-one.co.jp/h2gh/)
# ADULEDB-USBControll

## 細かなLEDの調整が可能！

![](https://bit-trade-one.co.jp/wp/wp-content/uploads/2019/08/c675e15c7065c2346c50e44bfd119b58.jpg)  

アプリ上からLEDの明るさを個別に細かく制御したり、高速に点滅させることが可能です。  
PWMコントロールには32bitマイコンを使用しチラつきの無い点灯を実現。  
設定した明るさを即座に反映します。    
センサ反応をLED制御のトリガーとすることで、様々な状況に応じてLEDを制御することができます。  

**ご注意！**  
本製品をお使いになるには電子工作や電子回路についての一般的な知識が必要です。  
LED本体は付属しません。  
LED点灯用の外部電源は付属しません。  

## [製品HPはこちらから](https://bit-trade-one.co.jp/aduledb/) 

# PC制御アプリ

### [アプリケーションソフト-ダウンロードリンク](https://github.com/bit-trade-one/ADUBRU-RelayControll/raw/master/PC-Tool/USB_Relay_Controll_CT_5Relay.exe)  

#### [アプリケーションソフト・ソース](https://github.com/bit-trade-one/ADULEDB-USBControll/tree/master/PC-Tool)  

---
## ライブラリ

### [C#ライブラリ](https://github.com/bit-trade-one/ADULEDB-USBControll/tree/master/Library-Cs)

### [C++ライブラリ](https://github.com/bit-trade-one/ADULEDB-USBControll/tree/master/Library-Cpp)

### [Visual Basicライブラリ](https://github.com/bit-trade-one/ADULEDB-USBControll/tree/master/Library-VB)
---

## 回路図

### [回路図](https://github.com/bit-trade-one/ADULEDB-USBControll/blob/master/Schematics/usbledcnt-gen_v11_20190627_sch.pdf)

#### [基板外形](https://github.com/bit-trade-one/ADULEDB-USBControll/blob/master/Schematics/ADULEDB%E5%9F%BA%E6%9D%BF%E5%A4%96%E5%BD%A2%E5%9B%B3.pdf)

#### [基板図](https://github.com/bit-trade-one/ADULEDB-USBControll/blob/master/Schematics/usbledcnt-gen_v11_20190627_brd.pdf)
---


## ファームウェア

### [ファームウェア-ダウンロードリンク](https://github.com/bit-trade-one/ADULEDB-USBControll/raw/master/Firmware/FW_LEDController_v100.zip)

### [ファームウェアアップデートツール-ダウンロードリンク](https://github.com/bit-trade-one/ADULEDB-USBControll/raw/master/Firmware/USBLEDController_UpdateTool.exe)

#### [ファームウェアソース](https://github.com/bit-trade-one/ADULEDB-USBControll/tree/master/Firmware)

---


## 製品仕様

基本仕様  
【入力】  
LED電源：  
・外部(DC15V以下)またはUSBから供給(DC5V)を選択可能（基板上のジャンパーピンで切替）  
・外部電源はDCジャックまたは端子台のどちらかを使用可能（極性に注意すること）  
　DCジャック：外形5.5mm／内径2.1mm、センタープラス  
※外部電源は使用者が用意すること、LEDの電圧および電流に合わせること  
※LEDの電源だけでは本製品は動作しない。本製品をPCのUSB端子に接続すること  
本体電源：USBから供給  
【LED出力】  
シンク型（オープンドレイン）  
LED電源（正極）  
端子：スルーホール(2.54mmピッチ、2X10)  
※スルーホールにLEDを直接ハンダ付けすること  
※市販のピンヘッダを取付可能（ハンダ付けが必要、ピンヘッダは使用者が用意すること）  
【LED仕様】  
・外部電源を使う場合：電圧15V以下、電流1A以下  
・USBからの電源(DC5V)を使う場合：電流50mA以下  
※必ず電流制限抵抗入りのLEDを使うこと（LEDや本製品に破損の恐れがあります）  
【周辺機能】赤外線受光部、LED、ブザー  
【インターフェイス】USB B  
【本体寸法】67×94.4×13mm（ハンダ面側の突起を含まず）  
【重量】約30g  
【使用温度】 0 ～ 40℃（結露なきこと）  
【生産国】Made in Japan  
