

# build-guide

|部品|個数|備考|
|:--|:--|:--|
|基板|1||
|[ダイオード(リードタイプ)](https://shop.yushakobo.jp/products/a0800di-01-100)|||
|[ウレタンクッション](https://shop.yushakobo.jp/products/a0800ur-01-6)||滑り止めとして底面に貼ります。|
|[ウレタンクッション(5mm厚)](https://www.yodobashi.com/product-detail/100000001003359892/)||滑り止めとして底面に貼ります。|
|[ネジ(M2 5mm)](https://shop.yushakobo.jp/products/a0800n2?variant=37665432993953)|||
|短いネジ(M2 6mm)|12||
|長いネジ(M2 10mm)|12||
|[ナット(M2)](https://shop.yushakobo.jp/products/4094)|12||
|[スペーサー(M2 nミリ以上)](https://shop.yushakobo.jp/products/a0800c2)|||
|[RP2040-Zero](https://talpkeyboard.net/items/640ea9f3072c3c538731c515)|||
|[ロータリーエンコーダ](https://shop.yushakobo.jp/products/3762)|||
|[小型アナログジョイスティック](https://www.switch-science.com/products/2892?srsltid=AfmBOorPHoOU9B2cyXs_Br7kAcbDDWK3j9G4ZUs7ezuBqDBhf63sDdMf)|||
|[キースイッチソケット(MX)](https://shop.yushakobo.jp/products/a01ps)||キースイッチの取り替えが用意になります。|
|[キースイッチソケット(Choc)](https://shop.yushakobo.jp/products/a01ps?variant=37665172553889)||キースイッチの取り替えが用意になります。|
|[Cherry MX互換キースイッチ](https://shop.yushakobo.jp/collections/all-switches)|||

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

