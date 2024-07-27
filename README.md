# BinsPack-for-StackChan-Core2

SD-Updaterに対応したスタックチャン(Core2版)のBINファイル集です。<br>
スタックチャン用ソフト８種とランチャー(menu.bin) ＋ ツール（２）＋おまけ（１）を同梱しています。

各ソフトの内容は、リンクをご参照ください。

## BINS

"Copy-to-SD"フォルダ下にSDで使用するファイルがあります。<br>

- [01_btSpeaker.bin](https://github.com/NoRi-230401/SDU-stackchan-bluetooth-simple)<br>
  Bluetooth Speaker<br>
  レベルメーターやFaceチェンジ機能付き<br>
※SDの yaml/SC_Config.yaml の設定ファイルを使用します。<br>
Bluetoothスピーカー名・起動時ボリューム等を変更することができます。<br>
<br>

- [02_radiko.bin](https://github.com/NoRi-230401/SDU-M5Unified_StackChan_Radiko)<br>
Radiko<br>
WebRadio Radikoプレイヤー付きのスタックチャン<br>
<b>"servo.txt"で、サーボ設定。(2024-06-05更新)</b><br>
<br>

- [03_wss.bin](https://github.com/NoRi-230401/WebServer-with-stackchan)<b>--- New（2024-07-11)</b><br>
  WebServer-with-Stackchan<br>
  2024-07-11 rootCACertificate.h更新しました。<br>
  AiStackChan2相当、サーボ調整、リモコン等たくさんの機能を詰め込みました。<br><br>

- [04_whisperMp3.bin](https://github.com/NoRi-230401/SDU-M5Unified_StackChan)<br>
  stackchan-whisper-mp3<br>
  スタックチャンが独り言を言います。セリフをSDカードにmp3ファイルで入れておくとランダムに再生します。<br>
  通信環境(WiFi等)がいらないソフトなので気楽に使えます。デモや販促等で活躍できそうです。<br>
  mp3のデータファイルと"servo.txt","volume.txt"の設定ファイルを使用します。<br>
  <br>

- [05_avatarLite.bin](https://github.com/NoRi-230401/SDU-M5Core2ImageAvatarLite)<br>
  Image Avatar Lite<br>
独自Avatar開発の為のソフトウエア・ツールです。<br>
Avatarが、サーボ・LED・bluetoothスピーカ音声とコラボして変化します。<br>
<br>

- [06_tester.bin](https://github.com/NoRi-230401/SDU-stack-chan-tester)<br>
  stack-chan-tester<br>
  スタックチャンを作成するときに、PWMサーボの調整及びテストを行うためのソフト。<br>
  "servo.txt"で、サーボPIN設定をします。<br>
<br>

- [07_AiStackChan2.bin](https://github.com/NoRi-230401/SDU-AI_StackChan2)<b>--- New（2024-07-11)</b><br>
  AiStackChan2<br>
  2024-07-11 rootCACertificate.h更新しました。<br>
  robo8080さんの AiStackChan2を SD-Updater対応しました。<br>
  "servo.txt"で、サーボ設定をします。<br>
 <br>

- [08_avatarMic.bin](https://github.com/NoRi-230401/SDU-m5stack-avatar-mic)<br>
  Avatar-Mic<br>
  Micで拾った音に合わせてAvatarが口パクしたり、傾いたりします。<br>
  スタックチャンといつまでもいっしょにいたくなる、とっても楽しいソフトです。
<br>
<br>

<b>※01・02・07は、robo8080さんのソフトをSD-Updater対応したものです。</b><br>


<b>※04・05・06・08は、mongonta0716さんのソフトをSD-Updater対応したものです。</b><br>
<br>


- [menu.bin](https://github.com/tobozo/M5Stack-SD-Updater/releases)<br>
SD-Updaterのランチャーソフト。<br>
"M5Core2-Launcher-2.0.13.bin" を "menu.bin"に名前を変更したものです。
<br><br>

ツール<br>

- [00_WebDav.bin](https://github.com/NoRi-230401/SDU-WebDav)　<b>--- New（2024-06-21）</b><br>
  WebDav<br>
  SD-Updaterに対応したファイル管理（WebDav）ツールです。<br>
  PC等から直接、M5Stack Core2のSD/SPIFFSにアクセスすることができるようになります。<br>
  ファイルのコピー・変更・削除が簡単になります。<br>


<br>

- [91_imgView.bin](https://github.com/NoRi-230401/SDU-ImageViewer)　<b>--- New（2024-07-21）</b><br>
  Image Viewer<br>
  画像ファイル表示ツール<br>
  "/Pictures"フォルダ内の 「jpg/png形式」の画像ファイルを表示。<br>
  最大５０枚。フォルダは、設定ファイルで変更可能です。<br>
  ManualモードとAutoモードがあり、いろいろと表示順の変更ができます。<br>
　"/Pctures"フォルダに表示する画像データ、 および<br>
　"/app/imgView/imgView.json"　設定ファイルを設置してください。<br>
<br>

おまけ<br>

- [99_powerOff.bin](https://github.com/NoRi-230401/SDU-powerOff)<br>
  Power OFF<br>
  起動すると２０秒後に電源OFFするだけのソフト。<br>
  電源ボタンが壊れた人（私。。）にとって、必要なソフト<br>
  必要ない方は、SDに入れなくていいと思います。<br>
<br><br>




## 設定ファイル
SD直下に置いてください。

- servo.txt<br>
 02・04・05・06・07 で使用するServo設定ファイル<br>
１行目(USE_SERVO)： "on" または、 "off"<br>
２行目(SERVO_PIN_X) ： "13"(PortC)　または、"33"(PortA)<br>
３行目(SERVO_PIN_Y) ： "14"(PortC)　または、"32"(PortA)<br>
サーボを使用しない場合は、１行目を "off"　<br>
サーボを使用する場合は、　１行目を "on"　<br>
<br>

- led.txt<br>
05 で使用するLED設定ファイル<br>
１行目(USE_LED)： "on" または、 "off"<br>
LEDを使用しない場合は、 "off"<br>
LEDを使用する場合は、 　"on"　<br>
<br>

- volume.txt<br>
  04 で使用するVolume設定ファイル　（ 0 to 255 ）<br>
  <br>
  
- wifi.txt<br>
  00・02・03・07 で使用するWiFi設定<br>
  １行目：YOUR_WIFI_SSID<br>
  ２行目：YOUR_WIFI_PASS<br>
  設定テンプレート・ファイルを自分用に変更してSD直下にコピーしてください。<br>
  <br>

- apikey.txt<br>
  03・07 で使用するApiKey設定のテンプレート・ファイル<br>
  １行目：YOUR_OPENAI_APIKEY<br>
  ２行目：YOUR_VOICEVOX_APIKEY<br>
  ３行目：YOUR_STT_APIKEY<br>
  設定テンプレート・ファイルを自分用に変更してSD直下にコピーしてください。<br>
<br>
<br>
- <b>その他に、ソフト毎に設定またはデータファイル等が必要になるものがあります。<br>
各ソフトのリンク先の説明書を見てご確認ください。</b><br>
<br>
(例)<br>
01 は、yaml/SC_config.yamlファイルを使用します。<br>
04 は、mp3フォルダ下に音声データを使用します。<br>
05 は、bmp_xxxフォルダおよび jsonフォルダ下にデータが必要です。<br>
<br><br>



## 対応ハードウエア
### 本体:　 M5Sstack Core2
- M5Stack Core2 for AWS（動作確認している機種）<br>
- M5Stack Core2 <br>
- ~~M5Stack Core2 v1.1~~　<b>(menu.binが未対応 :2024-06-23追記)</b><br>
<br>

### サーボ：SG90とその互換機種
- サーボなしの場合は、servo.txt の1行目を"off"にしてください。<br>
- サーボポートは、PortAまたは、PortC のどちらにも対応。<br>
<br>

## インストール方法
- BINファイルは、全てSD直下にコピーしてください。<br>
- 設定ファイル(wifi.txt等)を、必要に応じて修正しSDにコピーしてください。<br>
- jpg / jsonフォルダ下のファイルをコピーするとmenu.binで対応ソフトの画像と説明が表示されます。<br>
<br>

### SD-Updaterが初めての場合には、M5stack Core2本体に一度だけSD-Updater対応のソフト（ファームウエア）を書き込む必要があります。<br>
次の２つの方法があります。<br>

- いずれかのソフトで、リンク先のGitHubからファイルを取得し、VsCodeの開発環境を整えコンパイルして、ファームウエアをCore2本体に書き込む。<br>

- M5Burnerを使用してWebServer-with-Stackchanのソフトを書き込む<br>
（簡単なのでこちらの方法を推奨）<br>
<br>

## 動作
電源投入直後のブート時に SD-UpdaterのLobby画面が現れます。<br>

- <b>"Skip >>"</b>　を押下、または、タイムアウト<br>
現在のソフトがそのまま起動して、初期化が開始されます。<br><br>
![画像](images/wss-sdupdater.jpg)<br><br>

- <b>"< Menu"</b>　を押下<br>
ランチャー・ソフト（menu.bin）が起動します。<br>
ここで、複数個のソフトから起動するソフトを選択することができます。<br>
![画像](images/IMG_menu.jpg )<br>

<br><br>
## SD-Updaterについて
tobozoさん開発。SDに複数のBINファイルを入れて、ソフトを切替えて使用できるようになります。<br>

https://github.com/tobozo/M5Stack-SD-Updater<br><br>


KeiYouのソフトの館：「M5Stack-SD-UpdaterでSDカードからアプリを起動！」<br>
https://progkeiyou.com/sd-updater1/<br><br>


タカオさん、2023/7/29 ｽﾀｯｸﾁｬﾝ お誕生日会 2023のLTで、M5Stack-SD-Updaterの概要を説明した時のスライド<br>
https://speakerdeck.com/mongonta0716/sutatukutiyandefu-shu-apuriwoqie-riti-erutekunituku

<br><br><br>