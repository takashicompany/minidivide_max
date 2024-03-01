# miniDivide MAX

<img src = "https://github.com/takashicompany/minidivide_max/blob/master/images/01.jpg?raw=true" width = "600px" />

## 部品

### キットに含まれているもの
|部品|個数|備考|
|:--|:--|:--|
|PCB|2||
|[ダイオード(表面実装型)](https://shop.yushakobo.jp/collections/all-keyboard-parts/products/a0800di-02-100)|56||
|[タクタイルスイッチ](https://shop.yushakobo.jp/products/a0800ts-01-1)|2||
|TRRSソケット|2||
|ゴム足シール|8||
|[チップ積層セラミックコンデンサー](https://akizukidenshi.com/catalog/g/gP-02151/)|2|BLE Micro Proでの無線化の際に使用。|
|[電源スイッチ(MK12C02)](https://ja.aliexpress.com/item/32798526843.html)|2|BLE Micro Proでの無線化の際に使用。|
|[HU1632](https://www.monotaro.com/p/8835/2765/)|2|BLE Micro Proでの無線化の際に使用。|
|短いネジ(M2 4mm)|14||
|長いネジ(M2 8mm)|14||
|短いスペーサー(M2 4mm)|2||
|長いスペーサー(M2 8mm)|6||
|ナット(M2)|12||

### ご自身で用意頂くもの

**※2023/08/13よりアクリルケースはキットに同梱されておりません。**  
Boothにて「miniDivide アクリルケース」を追加で購入頂くか、[遊舎工房のキーボードアクリルプレート
から「miniDivide (Choc v1キースイッチ用) - 2mm」](https://shop.yushakobo.jp/products/keyboard_acrylic_plate?variant=46424950604007)をお求めください。  
遊舎工房キーボードアクリルプレートから発注頂きますと、お好みのカラーを選択することも可能です。

|部品|個数|備考|
|:--|:--|:--|
|スイッチプレート|2|2mm厚アクリルプレート。|
|側面プレート|2|2mm厚アクリルプレート。|
|ボトムプレート|2|2mm厚アクリルプレート。|
|Pro Microプレート|2||
|[Kailh Choc v1キースイッチ](https://shop.yushakobo.jp/collections/all-switches/products/pg1350)|38||
|0.8uキーキャップ(16mm)|38|詳細は後述|
|[Pro Micro](https://talpkeyboard.net/?category_id=59e2ad48c8f22c3720001301)|2|動作確認済みのものは[こちら](https://talpkeyboard.net/items/62e24e6f8a0bd07fe2d38137)|

### 組み立て方

工程自体はminiDivideと同様ですので、[miniDivideのビルドガイド](https://github.com/takashicompany/minidivide)を見ながら組み立ててください。

以下はminiDivideとの差分です。
作業に入る前に事前に目を通しておくことを推奨します。  

### リセットスイッチの取り付け

miniDivideのリセットスイッチは表面実装型のタクタイルスイッチを使用していますが、miniDivide MAXは2ピンのスルーホール型のタクタイルスイッチを使用します。  
取付箇所は両手ともにPro Micro取り付け位置の手前側です。  
<img src = "https://github.com/takashicompany/minidivide_max/blob/master/images/build/IMG_6001.JPG?raw=true" width = "600px" />

「RESET」と書かれている箇所にタクタイルスイッチを挿し込みます。  
<img src = "https://github.com/takashicompany/minidivide_max/blob/master/images/build/IMG_6002.JPG?raw=true" width = "600px" />

裏返してタクタイルスイッチの足が出ていることを確認します。  
<img src = "https://github.com/takashicompany/minidivide_max/blob/master/images/build/IMG_6003.JPG?raw=true" width = "600px" />

タクタイルスイッチの足と基板をハンダ付けします。  
<img src = "https://github.com/takashicompany/minidivide_max/blob/master/images/build/IMG_6004.JPG?raw=true" width = "600px" />

### ファームウェア

ファームウェアのソースコードは[こちら](https://github.com/qmk/qmk_firmware/pull/22804)。

[Remapにファームウェアを登録しております](https://remap-keys.app/catalog/45QFUzpwRR502dBTFs1W/firmware)ので、Webブラウザ上でファームウェアの書き込みとキーマップの変更が可能です。

### BLE Micro Proによる無線化

[こちら](https://github.com/takashicompany/BLE-Micro-Pro/tree/minidivide_max/v1/AboutDefaultFirmware/keyboards/takashicompany/minidivide_max)に、config.json(CONFIG.JSN)とkeymap.json(KEYMAP.JSN)があります。 近日中にプルリクエストを出す予定です。
