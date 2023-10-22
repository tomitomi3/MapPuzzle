# MapPuzzle
地図データから作る地図ジグソーパズル / Map Puzzle made from Shape data

## [市区町村パズル MFT2023ver](https://github.com/tomitomi3/MapPuzzle/tree/main/CityPuzzle_MFT2023)

Maker Faire Tokyo 2023で展示した47都道府県のSTLデータです。

[Shape2STL](https://github.com/tomitomi3/Shape2stl)を使用してShapeデータをSTLに変換しています。

### 概要

* 地図の投影にアルベルス正積円錐図法を用いています。
* 各都道府県のパズルのSTLデータは、外接する矩形の1辺が20cmとなるように設定しています。
* STLデータは県毎に2つあります。
  * [県コード]_ [都道府県名] _[～略～].stl 地図パズル本体
  * [県コード]_ [都道府県名] _[～略～]_wakubottom.stl 地図パズルの枠

### 3Dプリンタ パラメータ

Curaの設定を下記にして印刷しています。

* レイヤー厚 0.2 mm
  * <img src="img\3dprinter_setting_3.PNG">
* 初期水平展開（1層目の水平展開）を-0.1 mm
  * <img src="img\3dprinter_setting_1.PNG">
* ビルドプレート スカート
  * <img src="img\3dprinter_setting_2.PNG">

### 地図データの出展

国土数値情報 行政区域 第3.1版（ https://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-N03-v3_1.html ）を加工して作成しています。
