# BinsPack-for-StackChan-Core2

SD-Updaterに対応したスタックチャン(Core2版)のBINファイル集です。<br>
スタックチャン用ソフト３種とランチャー(menu.bin)を同梱しています。

ソフト本体の内容は、下記のリンクをご参照ください。

## BINS

- [01-wss.bin](https://github.com/NoRi-230401/WebServer-with-stackchan)<br>
  WebServer-with-Stackchan

- [02-radiko.bin](https://github.com/NoRi-230401/SDU-M5Unified_StackChan_Radiko)<br>
Radiko

- [03-btSpeaker.bin](https://github.com/NoRi-230401/SDU-stackchan-bluetooth-simple)<br>
  Bluetooth Speaker

<b>※02および03は、robo8080さんのソフトを変更して、SD-Updaterに対応しました。</b><br>
<br>
- [menu.bin](https://github.com/tobozo/M5Stack-SD-Updater/releases)<br>
SD-Updaterのランチャーソフト。<br>
"M5Core2-Launcher-2.0.13.bin" を "menu.bin"に名前を変更したものです。
<br><br>

## その他のファイル
- wifi.txt<br>
  "01-wss.bin"および "02-radiko.bin"で使用するWiFi設定のテンプレート・ファイル<br><br>
- apikey.txt<br>
  "01-wss.bin"　ApiKey設定のテンプレート・ファイル<br><br>
<br>

## 対応ハードウエア
- M5Stack Core2 for AWS<br>
- M5Stack Core2 <br>
- M5Stack Core2 v1.1　（未確認）<br><br>

## インストール方法
- BINファイルは、全てSD直下にコピーしてください。<br>
- 設定ファイル(wifi.txt等)は、必要に応じて修正してからSDにコピーしてください。<br>
- jpg / jsonフォルダ下のファイルをコピーするとソフト画像と説明が表示されます。<br>

SD-Updaterが初めての場合には、Core2本体に一度だけソフトを書き込む必要があります。<br>
Githubでファイルを取得しVsCodeを使用してコンパイル後に書き込むこともできますが、<br>
<b>簡単なのは、M5Burnerを使用してWebServer-with-Stackchanのソフトを書き込むこともできます。</b><br>
一度ソフトを書き込んだ後は、いつでもソフトを切替えて使用することができます。<br>
<br><br>

## ブート時
ブート時には SD-UpdaterのLobby画面が表示されます。<br>

- <b>"Skip >>"</b> 選択または、タイムアウトで、前回動作したソフトがそのまま起動します。<br><br>
![画像](images/wss-sdupdater.jpg)<br>

- <b>"< Menu"</b>  押下するとソフト選択(ランチャー)に移動。（次の画像）<br>
<br>ここで、起動ソフトを選択することができます。<br>
![画像](images/IMG_menu.jpg )<br>

<br><br>
## SD-Updaterについて
tobozoさん開発。SDに複数のBINファイルを入れて、ソフトを切替えて使用できるようになります。<br>

 https://github.com/tobozo/M5Stack-SD-Updater<br><br>


タカオさん、2023/7/29 ｽﾀｯｸﾁｬﾝ お誕生日会 2023のLTで、M5Stack-SD-Updaterの概要を説明した時のスライド
https://speakerdeck.com/mongonta0716/sutatukutiyandefu-shu-apuriwoqie-riti-erutekunituku