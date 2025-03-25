# ビルドガイドのテンプレート

ビルドガイドのテンプレートをつくるのがこのリポジトリの目的。

---

# build-guide
![image](https://github.com/user-attachments/assets/7905ab65-cbd3-40fc-ad86-46748c8f58a2)

|画像|部品|個数|備考|
|:--|:--|:--|:--|
||基板|1||
|<img src = "https://github.com/user-attachments/assets/79aed986-e14c-405d-bb84-741b5c8830ee" width = "200px" />|[ダイオード(リードタイプ)](https://shop.yushakobo.jp/products/a0800di-01-100)|||
|<img src = "https://github.com/user-attachments/assets/7905ab65-cbd3-40fc-ad86-46748c8f58a2" width = "200px" />|[ダイオード(SMDタイプ)](https://shop.yushakobo.jp/products/a0800di-02-100)|||
||[タクタイルスイッチ - 2pin 3.5x6x4.3mm](https://shop.yushakobo.jp/products/a0800ts-01-1)||ファームウェアを書き込む際に使用します。|
||[ウレタンクッション](https://shop.yushakobo.jp/products/a0800ur-01-6)||滑り止めとして底面に貼ります。|
||[ウレタンクッション(5mm厚)](https://www.yodobashi.com/product-detail/100000001003359892/)||滑り止めとして底面に貼ります。|
||[ネジ(M2 5mm)](https://shop.yushakobo.jp/products/a0800n2?variant=37665432993953)|||
||短いネジ(M2 6mm)|12||
||長いネジ(M2 10mm)|12||
||[ナット(M2)](https://shop.yushakobo.jp/products/4094)|12||
||[スペーサー(M2 nミリ以上)](https://shop.yushakobo.jp/products/a0800c2)|||
|<img src = "https://github.com/takashicompany/rookey/assets/4215759/1fe9f782-f64b-4291-b03c-e1532b05013b" width = "200px" />|[Pro Micro](https://shop.yushakobo.jp/products/21)||MCU(Micro Controller Unit)というキーボードの頭脳部分です。|
||[コンスルー](https://shop.yushakobo.jp/products/31?variant=37665714372769)|||
||[RP2040-Zero](https://talpkeyboard.net/items/640ea9f3072c3c538731c515)||MCU(Micro Controller Unit)というキーボードの頭脳部分です。|
||[ロータリーエンコーダ](https://shop.yushakobo.jp/products/3762)|||
||[小型アナログジョイスティック](https://www.switch-science.com/products/2892?srsltid=AfmBOorPHoOU9B2cyXs_Br7kAcbDDWK3j9G4ZUs7ezuBqDBhf63sDdMf)|||
||[キースイッチソケット(MX)](https://shop.yushakobo.jp/products/a01ps)||キースイッチの取り替えが用意になります。|
||[キースイッチソケット(Choc)](https://shop.yushakobo.jp/products/a01ps?variant=37665172553889)||キースイッチの取り替えが用意になります。|
||[Cherry MX互換キースイッチ](https://shop.yushakobo.jp/collections/all-switches)|||

## 組み立てに必要な道具

何を用意してよいか分からない方は、[こちら](https://shop.yushakobo.jp/products/a9900to)を購入するのが確実です。

|道具|備考|
|:--|:--|
|ハンダごて|おすすめは[HAKKO FX-600](https://www.hakko.com/japan/products/hakko_fx600.html)です。[こて台](https://www.hakko.com/japan/products/hakko_kote_board.html)もあると、より作業をスムーズに進められます。|
|ハンダ|[こちら](https://www.goot.jp/products/detail/se_06008)などを使う方が多いようです。|
|ピンセット|100均などで手に入るものでも充分利用できるかと思います。|
|ニッパー|100均などで手に入るものでも充分利用できるかと思いますが、1000円程度ものを買っても損では無いかと思います。|

## あるとさらに完成度が高くなる道具
|道具|備考|
|:--|:--|
|棒ヤスリ|基板の縁にあるバリを削るのに使います。|
|サインペン|基板の縁を塗るとより美しくなります。|
|マスキングテープ|キースイッチをハンダ付けする際に役立ちます。|

# 組み立て方

## 1. 基板の表裏を確認する

### 表
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/010-01.jpg?raw=true" width = "600px" />

### 裏
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/010-02.jpg?raw=true" width = "600px" />

## 2. ダイオードのハンダ付け

基板にダイオードをハンダ付けします。ダイオードはキースイッチを押下した際に電流をMCUに伝達する役目を持ちます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/020-diode-a-01.jpg?raw=true" width = "600px" />

ダイオードは基板の裏側から取付けます。ダイオードの配置箇所の「`▷|`」の縦線とダイオードの黒い線の方向が同じになるように置きます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/020-diode-a-02.jpg?raw=true" width = "600px" />

ダイオードが基板の穴を通るように足を折り曲げます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/020-diode-a-03.jpg?raw=true" width = "600px" />

ダイオードの足を基板に通します。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/020-diode-a-04.jpg?raw=true" width = "600px" />

反対側からダイオードの足が出ていることを確認します。
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/020-diode-a-05.jpg?raw=true" width = "600px" />

基板とダイオードの足をハンダ付けします。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/020-diode-a-06.jpg?raw=true" width = "600px" />

ハンダ付けした後にダイオードの足をニッパーなどで切ります。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/020-diode-a-07.jpg?raw=true" width = "600px" />

## 3. MCUの取付け

MCU(Micro Controller Unit)は簡単に説明するとキーボードの頭脳部分です。キースイッチ等の入力を処理してPC等に伝達します。  

当キーボードでは、Waveshare RP2040-Zeroを使用します。  
<img src = "https://github.com/user-attachments/assets/f00b9381-6d04-48e2-aeb9-90fa7b754eb1" width = "600px" />

下図の位置にMCUを置きます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/040-rp2040-zero-02.jpg?raw=true" width = "600px" />

基板のハンダ付けの銀箔とMCUのハンダ付け箇所が合致するように位置合わせを行います。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/040-rp2040-zero-03.jpg?raw=true" width = "600px" />

基板とMCUをハンダ付けします。置き場所がズレていないかを随時確認しながらハンダ付けを行います。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/040-rp2040-zero-04.jpg?raw=true" width = "600px" />

全部で23箇所をハンダ付けしたら完了です。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/040-rp2040-zero-05.jpg?raw=true" width = "600px" />

## 6. キースイッチソケットの取付け

キースイッチソケットは基板とキースイッチを接続するものです。この部品を用いることでキースイッチ自体を基板にハンダ付けする必要がなくなるのでキースイッチの交換が容易になります。  

<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/060-switch-socket-01.jpg?raw=true" width = "600px" />

キースイッチソケットは基板の裏側に取付けます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/060-switch-socket-02.jpg?raw=true" width = "600px" />

基板にあるキースイッチハンダ付け箇所の片側にハンダを載せておきます。([予備ハンダ](https://www.p-ban.com/htmlmail_qanda/2019/12/))  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/060-switch-socket-03.jpg?raw=true" width = "600px" />

キースイッチソケットをピンセットで持ちながら予備ハンダを溶かしながらソケットの片側と基板をハンダ付けします。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/060-switch-socket-04.jpg?raw=true" width = "600px" />

もう片方もハンダ付けをします。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/060-switch-socket-05.jpg?raw=true" width = "600px" />

## 7. キースイッチとプレートの取付け

スイッチプレートに保護シートがある場合は剥がしてください。アクリル板の場合は水を少量つけてピンセットで端を持つと剥がれやすいことがあります。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/070-switch-01.jpg?raw=true" width = "600px" />

基板の上にスイッチプレートを載せます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/070-switch-02.jpg?raw=true" width = "600px" />

キースイッチを用意します。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/070-switch-03.jpg?raw=true" width = "600px" />

<!--
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/070-switch-04-js-01.jpg?raw=true" width = "600px" />


<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/070-switch-04-js-02.jpg?raw=true" width = "600px" />


<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/070-switch-04-js-03.jpg?raw=true" width = "600px" />
-->

数個のキースイッチをスイッチプレートに挿し込んで、基板とスイッチプレートをキースイッチで仮止めします。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/070-switch-04.jpg?raw=true" width = "600px" />

全てのキースイッチを取付けます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/070-switch-07.jpg?raw=true" width = "600px" />

## 7b. ロータリーエンコーダの取付け

ロータリエンコーダは回転操作による入力が可能です。スクロール操作によく使われます。ロータリーエンコーダによっては押し込みによりキー入力が可能なものもあります。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/071-rotary-01.jpg?raw=true" width = "600px" />

基板の表面にロータリーエンコーダーを差し込みます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/071-rotary-02.jpg?raw=true" width = "600px" />

基板の裏側からロータリーエンコーダの足が出ていることを確認します。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/071-rotary-03.jpg?raw=true" width = "600px" />

ロータリーエンコーダの足と基板をハンダ付けしたら完了です。
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/071-rotary-04.jpg?raw=true" width = "600px" />

## 8. ボトムプレートの取付け

ボトムプレートに保護シートがある場合は剥がしてください。アクリル板の場合は水を少量つけてピンセットで端を持つと剥がれやすいことがあります。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/080-bottom-01.jpg?raw=true" width = "600px" />

スペーサーとネジを使用してボトムプレートとスイッチプレートを固定します。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/080-bottom-02.jpg?raw=true" width = "600px" />

ボトムプレートの底面側からネジ穴にネジを挿します。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/080-bottom-03.jpg?raw=true" width = "600px" />

ボトムプレートの上面側から挿したネジをスペーサーで固定します。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/080-bottom-04.jpg?raw=true" width = "600px" />

ボトムプレートの上に基板とスイッチプレートを重ねます。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/080-bottom-05.jpg?raw=true" width = "600px" />

スペーサーとスイッチプレートをネジで固定します。  
<img src = "https://github.com/takashicompany/keyboard-name-here/blob/master/images/build/080-bottom-06.jpg?raw=true" width = "600px" />


### xx. 完成した後の楽しみ方

完成しましたら、ぜひSNSなどに写真を投稿頂ければと思います。
Twitterのハッシュタグは [`#キーボード名 #自作キーボード`](https://twitter.com/search?q=%23%E8%87%AA%E4%BD%9C%E3%82%AD%E3%83%BC%E3%83%9C%E3%83%BC%E3%83%89%20%23キーボード名&src=typed_query) を付けていただけると幸いです。
キットを組み立てた感想や、キーボードを使った所感などをお待ちしております！

また、毎週日曜日の１9時より実施されている[#KEEP_PD](https://twitter.com/hashtag/KEEB_PD?f=live)に投稿頂くこともオススメです。  
開催の告知は[@KEEB_PD](https://twitter.com/KEEB_PD)にて行われております。

ご不明な点などございましたら、[@takashicompany](https://twitter.com/takashicompany)にメンションやDM頂ければ回答できるかと思います。

