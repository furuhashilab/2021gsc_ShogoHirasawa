## Introduction:
What are you studying and why? 何を研究したのか？ 何故それを研究したのか？(500文字以内で簡単に記述する)



## Methods:
次の3つの工程に分けて実装を行った。1.UNVT Portabl アクセスポイント化 2.タイルデータの制作 3.htmlファイルの実装。この章では各工程の実装の手法を紹介する。   
* UNVT Portabl アクセスポイント化

MacとUNVT PortableをEthernetケーブルで有線接続している状態で、実装に着手した。最初に以下のパッケージ5つ（apatch2、hostapd、dnsmasq、isc-dhcp-server、rng-tools）をインストールし、その後にUNVT PortableのIPアドレスの固定化、Wi-FiのSSIDとPassの設定を行った。QRコード読み取りによるWi-Fi接続の簡便化も行い、特別な知識のない人でも、自分の所有する端末を用いて、オフライン環境下でデジタル地図をスマホやPCで閲覧可能とさせた。

* タイルデータの制作

二子玉川駅付近のWeb地図を制作した。本マップを表示するにあたり、次の4つのタイルデータ（道路ベクトルタイル・建物ベクトルタイル・二子玉川の空撮ラスタータイル・世田谷区避難所ベクトルタイル）を制作した。道路ベクトルタイル・建物ベクトルタイルはOpenStreetMap、二子玉川の空撮ラスタータイルはOpenAerialMap、世田谷区避難所ベクトルタイルは東京都オープンデータカタログサイトからデータを引用し、それをUNVTにも採用されているオープンソースソフトのTippicanueで用いてタイル化を行った。

* htmlファイルの実装

オフラインで機能するWeb地図アプリケーションを作成するため、MapLibre GL JSを使い実装を行った。上記で記載した、各タイルをSourceレイヤーで指定し、道路ベクトルタイル・建物ベクトルタイル・二子玉川の空撮ラスタータイル・世田谷区避難所ベクトルタイルの順で記述し、避難所データが最前面となるようLayersレイヤーに記述した。避難所のポイントデータは画像としてで表示させた。


## Results:
What did you find? 何がわかったのか? (500文字以内で簡単に記述する)



## Discussion:
What do your findings mean? あなたが見つけたことは何を意味するのか？どんな議論をしたか。(500文字以内で簡単に記述する)



## Conclusion:
What have you learned from the study? この研究を通じて得られたものは？次に引き継ぐべき課題は？(500文字以内で簡単に記述する)

## Reference/参考文献:
卒業論文本文中に記載。

## Acknowledgements/謝辞:
本研究を進めるにあたり〇〇〇の〇〇氏をはじめ多くの方々より多大な助言を賜りました。厚く感謝を申し上げます。

© FuruhashiLabratory/ShogoHirasawa, CC BY 4.0


    
