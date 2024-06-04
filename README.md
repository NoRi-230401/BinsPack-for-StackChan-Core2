# BinsPack-for-StackChan-Core2

SD-Updaterに対応したスタックチャン(Core2版)のBINファイル集です。<br>
スタックチャン用ソフト７種とランチャー(menu.bin) ＋ おまけ（１）を同梱しています。

各ソフトの内容は、リンクをご参照ください。

## BINS

"Copy-to-SD"フォルダ下にSDで使用するファイルがあります。<br>

- [01_btSpeaker.bin](https://github.com/NoRi-230401/SDU-stackchan-bluetooth-simple)<br>
  Bluetooth Speaker<br>
<br>

- [02_radiko.bin](https://github.com/NoRi-230401/SDU-M5Unified_StackChan_Radiko)<br>
Radiko<br>
WebRadio Radikoプレイヤー付きのスタックチャン


- [03_wss.bin](https://github.com/NoRi-230401/WebServer-with-stackchan)<br>
  WebServer-with-Stackchan<br>
  AiStackChan2相当、サーボ調整、リモコン等たくさんの機能を詰め込みました。<br><br>

- [04_whisperMp3.bin](https://github.com/NoRi-230401/SDU-M5Unified_StackChan)<br>
  stackchan-whisper-mp3<br>
  スタックチャンが独り言を言います。セリフをSDカードにmp3ファイルで入れておくとランダムに再生します。<br>
  通信環境(WiFi等)がいらないソフトなので気楽に使えます。デモや販促等で活躍できそうです。<br>
  mp3のデータファイルと"servo.txt","volume.txt"の設定ファイルを使用します。<br>
  実行前にSDにコピーが必要です。
<br><br>

- [05_AvatarLite.bin](https://github.com/NoRi-230401/SDU-M5Core2ImageAvatarLite)<br>
  Image Avatar Lite<br>
独自Avatar開発の為のソフトウエア・ツールです。<br>
Avatarが、サーボ・LED・bluetoothスピーカ音声とコラボして変化します。<br>
<br>

- [06_tester.bin](https://github.com/NoRi-230401/SDU-stack-chan-tester)<br>
  stack-chan-tester<br>
  スタックチャンを作成するときに、PWMサーボの調整及びテストを行うためのソフト。<br>
  外部ファイル("servo.txt")で、サーボPIN設定をします。<br>
<br>

- [07_AiStackChan2.bin](https://github.com/NoRi-230401/SDU-AI_StackChan2)<br>
  AiStackChan2<br>
  あのrobo8080さんの AiStackChan2を SD-Updater対応しました。<br>
  外部ファイル("servo.txt")で、サーボ設定ができます。<br>
<br>

<b>※01・02・07は、　robo8080さんのソフトをSD-Updater対応したものです。</b><br>


<b>※04・05・06は、　mongonta0716さんのソフトをSD-Updater対応したものです。</b><br>
<br>


- [menu.bin](https://github.com/tobozo/M5Stack-SD-Updater/releases)<br>
SD-Updaterのランチャーソフト。<br>
"M5Core2-Launcher-2.0.13.bin" を "menu.bin"に名前を変更したものです。
<br><br>

おまけ<br>
- [00_powerOff.bin](https://github.com/NoRi-230401/SDU-powerOff)<br>
  Power OFF<br>
  起動すると２０秒後に電源OFFするだけのソフト。<br>
  電源ボタンが壊した人（私。。）にとって、必要なソフト<br>
  必要ない方は、SDに入れなくていいと思います。<br>
<br><br>




## 設定ファイル
SD直下に置いてください。

- servo.txt<br>
 04・05・06・07 で使用するServo設定ファイル<br>
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
  02・03・07 で使用するWiFi設定のテンプレート・ファイル<br>
  設定を自分用に変更してSD直下にコピーしてください。<br>
  <br>

- apikey.txt<br>
  03・07 で使用するApiKey設定のテンプレート・ファイル<br>
  設定を自分用に変更してSD直下にコピーしてください。<br>
<br>

## 対応ハードウエア
### 本体:　 M5Sstack Core2
- M5Stack Core2 for AWS（動作確認している機種）<br>
- M5Stack Core2 <br>
- M5Stack Core2 v1.1　<br>
<br>

### サーボ：SG90とその互換機種
- サーボなしの場合は、servo.txt の1行目を"off"にしてください。<br>
- サーボポートは、PortAまたは、PortC のどちらにも対応。<br>
<br>

## インストール方法
- BINファイルは、全てSD直下にコピーしてください。<br>
- 設定ファイル(wifi.txt等)は、必要に応じて修正してからSDにコピーしてください。<br>
- jpg / jsonフォルダ下のファイルをコピーすると対応ソフトの画像と説明が表示されます。<br><br>
- その他に、ソフト毎に独自にデータファイル等が必要になるものがあります。ソフトの説明書を見て確認してください。<br>
(例)<br>
04 は、mp3フォルダ下に音声データが必要です。<br>
05 は、bmp_xxxフォルダおよび jsonフォルダ下にデータが必要です。<br>
<br><br>


SD-Updaterが初めての場合には、Core2本体に一度だけ対応ソフト（ファームウエア）を書き込む必要があります。<br>
次の２つの方法があります。<br>

- 00～07 いずれかのソフトをGitHubでファイルを取得し、VsCodeの開発環境を整えコンパイルしてCore2本体に書き込む。<br>

- <b>M5Burnerを使用してWebServer-with-Stackchanのソフトを書き込む<br>
（簡単なのでこの方法を推奨します）</b>
<br><br>

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


タカオさん、2023/7/29 ｽﾀｯｸﾁｬﾝ お誕生日会 2023のLTで、M5Stack-SD-Updaterの概要を説明した時のスライド<br>
https://speakerdeck.com/mongonta0716/sutatukutiyandefu-shu-apuriwoqie-riti-erutekunituku

<br><br><br>