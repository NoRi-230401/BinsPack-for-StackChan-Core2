# BinsPack-for-StackChan-Core2

SD-Updaterに対応したスタックチャン(Core2版)のBINファイル集です。<br>
スタックチャン用ソフト４種とランチャー(menu.bin)を同梱しています。

各ソフトの内容は、リンクをご参照ください。

## BINS

"Copy-to-SD"フォルダ下にSDで使用するファイルがあります。<br>

- [01_btSpeaker.bin](https://github.com/NoRi-230401/SDU-stackchan-bluetooth-simple)<br>
  Bluetooth Speaker



- [02_radiko.bin](https://github.com/NoRi-230401/SDU-M5Unified_StackChan_Radiko)<br>
Radiko

<b>※01および02は、robo8080さんのソフトをSD-Updater対応したものです。</b><br>
<br>

- [03_wss.bin](https://github.com/NoRi-230401/WebServer-with-stackchan)<br>
  WebServer-with-Stackchan
<br><br>

- [04_whisperMp3.bin](https://github.com/NoRi-230401/SDU-M5Unified_StackChan)<br>
  stackchan-whisper-mp3<br>
  独り言を言うｽﾀｯｸﾁｬﾝです。セリフをSDカードにmp3ファイルで入れておくとランダムに再生します。<br>
  mp3のデータファイルと"servo.txt","volume.txt"の設定ファイルを使用します。<br>
  実行前にSDにコピーが必要です。
<br>

<b>※04は、@mongonta555 さんソフトをSD-Updater対応したものです。</b><br>
<br>


- [menu.bin](https://github.com/tobozo/M5Stack-SD-Updater/releases)<br>
SD-Updaterのランチャーソフト。<br>
"M5Core2-Launcher-2.0.13.bin" を "menu.bin"に名前を変更したものです。
<br><br>

## 設定ファイル
SD直下に置いてください。

- servo.txt<br>
  "04_whisperMp3.bin"で使用するServo設定ファイル<br>
  サンプル設定を添付しています。名前を"servo.txt"に変えてSD直下にコピー。<br>

- volume.txt<br>
  "04_whisperMp3.bin"で使用するVolume設定ファイル<br>
  サンプル設定を添付しています。<br>

- wifi.txt<br>
  "03_wss"および "02_radiko"で使用するWiFi設定のテンプレート・ファイル<br>
  設定を自分用に変更してSD直下にコピーしてください。<br>
  <br>

- apikey.txt<br>
  "03_wss.bin"　で使用するApiKey設定のテンプレート・ファイル<br><br>
  設定を自分用に変更してSD直下にコピーしてください。<br>
<br>

## 対応ハードウエア
- M5Stack Core2 for AWS（この機種で動作確認をおこなっています。）<br>
- M5Stack Core2 <br>
- M5Stack Core2 v1.1　<br><br>

## インストール方法
- BINファイルは、全てSD直下にコピーしてください。<br>
- 設定ファイル(wifi.txt等)は、必要に応じて修正してからSDにコピーしてください。<br>
- jpg / jsonフォルダ下のファイルをコピーすると対応ソフトの画像と説明が表示されます。<br><br>

SD-Updaterが初めての場合には、Core2本体に一度だけ対応ソフト（ファームウエア）を書き込む必要があります。<br>
次の２つの方法があります。<br>

- 01～03いずれかのソフトをGithubでファイルを取得し、VsCodeの開発環境を整えコンパイルしてCore2本体に書き込む。<br>

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