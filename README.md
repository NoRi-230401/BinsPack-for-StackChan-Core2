# BinsPack-for-StackChan-Core2

SD-Updaterに対応したスタックチャン(Core2版)のBINファイル集です。<br>
スタックチャン用ソフト３種とランチャー(menu.bin)を同梱しています。

ソフト本体の内容は、下記のリンクをご参照ください。

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
<br>

- [menu.bin](https://github.com/tobozo/M5Stack-SD-Updater/releases)<br>
SD-Updaterのランチャーソフト。<br>
"M5Core2-Launcher-2.0.13.bin" を "menu.bin"に名前を変更したものです。
<br><br>

## その他のファイル
- wifi.txt<br>
  "03_wss.bin"および "02_radiko.bin"で使用するWiFi設定のテンプレート・ファイル<br><br>
- apikey.txt<br>
  "03_wss.bin"　で使用するApiKey設定のテンプレート・ファイル<br><br>
<br>

## 対応ハードウエア
- M5Stack Core2 for AWS（これで動作確認しています。）<br>
- M5Stack Core2 <br>
- M5Stack Core2 v1.1　<br><br>

## インストール方法
- BINファイルは、全てSD直下にコピーしてください。<br>
- 設定ファイル(wifi.txt等)は、必要に応じて修正してからSDにコピーしてください。<br>
- jpg / jsonフォルダ下のファイルをコピーするとソフト画像と説明が表示されます。<br>
<br>
SD-Updaterが初めての場合には、Core2本体に一度だけ対応ソフトを書き込む必要があります。
次の２つの方法があります。<br>

- 01～03いずれかのソフトをGithubでファイルを取得し、VsCodeの開発環境を整えコンパイルしてCore2本体に書き込む。<br>

- <b>M5Burnerを使用してWebServer-with-Stackchanのソフトを書き込む（簡単なので推奨）</b>
<br><br>

## 動作
電源投入直後のブート時に SD-UpdaterのLobby画面が現れます。<br>

- <b>"Skip >>"</b> 選択または、タイムアウトで、現在のソフトがそのまま起動。<br><br>
![画像](images/wss-sdupdater.jpg)<br>

- <b>"< Menu"</b>  押下するとソフト選択(ランチャー)に移動。<br>
<br>ここで、複数ソフトから次に起動するものを選択することができます。<br>
![画像](images/IMG_menu.jpg )<br>

<br><br>
## SD-Updaterについて
tobozoさん開発。SDに複数のBINファイルを入れて、ソフトを切替えて使用できるようになります。<br>

 https://github.com/tobozo/M5Stack-SD-Updater<br><br>


タカオさん、2023/7/29 ｽﾀｯｸﾁｬﾝ お誕生日会 2023のLTで、M5Stack-SD-Updaterの概要を説明した時のスライド<br>
https://speakerdeck.com/mongonta0716/sutatukutiyandefu-shu-apuriwoqie-riti-erutekunituku

<br><br><br>