# 要旨
既存のDappsはオンラインゲームにおける様々な課題を解決してきたが、未だいくつか課題はのこる。
私たちはその中で「ゲームのサービスが終了してしまったときに何も残らない」という点を解決するために「プレーヤーが保持している他のゲームのアイテムの画像を集め使えるようなプラットフォーム」を提供する。

# 序説
既存のオンラインゲームはそのデータがゲーム運営元の管理するデータベースのみで保管されていることから、いくつかの課題を抱えている。
その課題に対してブロックチェーンをデータベースとして使用することは有用であり、様々なブロックチェーンを使った分散型アプリケーション（以下Dappsと呼ぶ）が開発されてきたが、まだいくつかの課題が残る。

## 既存のオンラインゲームの抱える課題

### 課題1:アイテムの売買や交換が運営元の管理下でしか行えない
オンラインゲームの市場はゲーム運営元が管理しており自由な交換が行えないものが多い。
特に今日のスマートフォン向けオンラインゲームでは交換や市場の機能が一切存在していないものが大多数である。
現実のトレーディングカードゲーム（以下TCGと呼ぶ）のようにプレイヤー間の自由な交換や売買ができる環境が望まれる。

### 課題2:サービス終了時にすべてのデータが消失してしまう
ゲームデータを運営元の管理するデータベースで保管している以上、その管理にはコストがかかりサービス終了時にはデータベースは削除され、そのデータは今後参照することができなくなってしまう。
しかしながら、オンラインゲームのデータにはプレイヤーの時間や資金がつぎ込まれているため、そのデータは存続し続けることが望ましい。

## 既存のDappsによる解決と未だ残る課題
既存のDappsにより、オンラインゲームが抱える課題のうちいくつかは解消されているが、いくつかの課題は未だ残る。
### アイテムの売買や交換が運営元の管理下でしか行えない問題への解決
現在最もDappsに用いられているプラットフォームはEthereumであり、Dappsで使われるアイテム（以下NFTアセットと呼ぶ）にはERC721という規格が用いられている。

ERC721の規格を用いることでブロックチェーン上でプレイヤーが所有しているアイテムはすべてゲーム外のマーケットで交換したり売買したりすることができるようになった。
現在さまざまな企業がNFTアセットのマーケットを運営しており取引も活発に行われている。

### サービス終了時にすべてのデータが消失してしまう問題への解決
データの保管場所としてブロックチェーンを選択することにより、サービスが終了してもデータはすべて存続するようになった。
ブロックチェーン上のデータは維持に特定の企業がコストを払う必要もないし、消そうとしても消せない性質をもっているからだ。
しかしながら、現在のDappsにおいてせっかくデータが残ってもそれを二次利用する場所がないのが現状である。

# 解決策
前述したとおり、既存のDappsにより多くのオンラインゲームの課題が解決されてきたが、「現在のDappsにおいてせっかくデータが残ってもそれを二次利用する場所がないのが現状である」という解決が未だ残っている
私たちは画像収集用Dappsとゲーム用のDappsを別途に開発することによりこの問題を解決する。

## 画像収集用Dapps
ブロックチェーン上のデータはすべて公開情報であるから、外部のAPIにより本人の所有するNFTアセットの画像を集めることが可能である。
画像収集用Dappsの目的は本人の所有するNFTアセットの画像をすべて収集して、後述するゲーム用Dappsで使えるようにすることである。
これにより、本人の所有するすべてのNFTアセットの画像は別のDappsゲームにおいても使うことが可能になる。
![flow](https://user-images.githubusercontent.com/16893450/65388679-27d46600-dd89-11e9-838a-774cb8ff052b.jpg)


## ゲーム用Dapps
本件において私たちはカードゲームを作成するが、誰でも上述の画像収集Dappsにより収集された画像を用いるゲームを作成することが可能である。

### カードゲームDapps
私たちの作成するカードゲームにおいて、プレイヤーが保持するNFTアセットはカードのステータス情報（以下フレームと呼ぶ）のみである。
そこにプレイヤーの保持する他のNFTアセットの画像を付加することによってカードが完成する。
このときにプレイヤーが使える画像は画像収集用Dappsによって集められたものであり、つまり本人の所有するNFTアセットである。
プレイヤーは本カードゲームにおけるNFTアセットであるフレームと自分の所有するNFTアセットの画像データを用いてカードを作成する。
そのカードを用いてデッキをつくってバトルすることや、自分独自のカードを売買・交換することができる。

# 結び
上述の通りたとえ他のDappsがサービス終了しても、その画像データはブロックチェーン上に残り続け、本件で作成する画像収集用Dappsにより様々な他のゲームで使えるようになる。
また本件では画像収集用Dappsを用いたゲームの第一弾としてカードゲームを作成する。


