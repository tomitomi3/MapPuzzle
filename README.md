# MapPuzzle
地図データから作る地図ジグソーパズル / Map Puzzle made from Shape data

[Shape2STL](https://github.com/tomitomi3/Shape2stl)を使用してShapeデータをSTLに変換しています。

## [MFT2023ver 47都道府県 市区町村ジグソーパズル](https://github.com/tomitomi3/MapPuzzle/tree/main/CityPuzzle_MFT2023)

Maker Faire Tokyo 2023で展示した47都道府県 市区町村ジグソーパズルのSTLデータです。

#### 補足

* 地図の投影にアルベルス正積円錐図法を用いています。
* 各都道府県のパズルのSTLデータは、外接する矩形の1辺が20cmとなるように設定しています。
* STLデータは県毎に2つあります。
  * [県コード]_ [都道府県名] _[～略～].stl 地図パズル本体
  * [県コード]_ [都道府県名] _[～略～]_wakubottom.stl 地図パズルの枠
* 印刷時は下部の[パラメータ](https://github.com/tomitomi3/MapPuzzle/tree/main#3d%E3%83%97%E3%83%AA%E3%83%B3%E3%82%BF%E3%83%91%E3%83%A9%E3%83%A1%E3%83%BC%E3%82%BF)参照

#### 地図データの出展

* 国土数値情報 行政区域 第3.1版（ https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-N03-v3_1.html ）を加工して作成しています。

## [YOXO2040 市区町村・町丁目ジグソーパズル](https://github.com/tomitomi3/MapPuzzle/tree/main/CityTownPuzzle_YOXO2024)

[YOXO FESTIVAL 2024](https://yoxo-o.jp/yoxofestival/)で展示した市区町村・町丁目ジグソーパズルのSTLデータです。

YOXOでは下記を展示しました。

* 石川県と富山県
* 神奈川県
* 神奈川県横浜市中区（会場が神奈川県 ハンマーヘッドだったため）
* 石川県の立体化

#### 補足

* 神奈川県横浜市中区は一部ポリゴンをマージしています。印刷時に小さくなることと四角の形状が多いためパズルとして難しいと判断したためです。
* 各都道府県のパズルのSTLデータは、外接する矩形の1辺が20cmとなるように設定しています。
* STLデータは県毎に2つあります。
  * ～略～_[都道府県名] _～略～.stl 地図パズル本体
  * ～略～_ [都道府県名] _～略～_wakubottom.stl 地図パズルの枠
* 印刷時は下部の[パラメータ](https://github.com/tomitomi3/MapPuzzle/tree/main#3d%E3%83%97%E3%83%AA%E3%83%B3%E3%82%BF%E3%83%91%E3%83%A9%E3%83%A1%E3%83%BC%E3%82%BF)参照

#### 地図データの出展

下記のデータを加工して作成しています。

* 国土数値情報 行政区域 第3.1版（ https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-N03-v3_1.html ）
* 令和２年国勢調査 町丁・字等境界データ 政府統計の総合窓口(e-Stat)（ https://www.e-stat.go.jp/ ）

## 3Dプリンタパラメータ

ジグソーパズル間のすき間を再現するために下記の設定を行っています（Curaの設定になります。）。3Dプリンタによって調整が必要かもしれません。

* レイヤー厚 0.2 mm
  * <img src="img\3dprinter_setting_3.PNG">
* 初期水平展開（1層目の水平展開）を-0.1 mm
  * <img src="img\3dprinter_setting_1.PNG">
* ビルドプレート スカート
  * <img src="img\3dprinter_setting_2.PNG">

