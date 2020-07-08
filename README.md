# まち歩きマップメーカー

## 目的・用途
印刷向けのまち歩き地図、案内地図、地図柄のグッズ制作などに使えるOpenStreetMap。  
でも、高機能だけど複雑なソフトウェアやプログラミングの知識は持っている人は少ない。  
  
そんな「パソコンでちょっとした文書は作れる程度」の方たちでも、もっと自由に地図を  
使って欲しいと思って、この「まち歩きマップメーカー」を開発しています。  
  
まち歩きマップメーカーを使うと、PNG/SVGという一般的な画像で地図のダウンロードが  
出来ます。あとは、プレゼンソフトでポップやアイコンを追加するだけで、お店や施設の  
案内地図や、まち歩きのイベントなどで配る地図を作ることが出来ます。  

## マニュアル
* [まち歩きマップメーカーのススメ](https://medium.com/@K_Sakanoshita/ea38ce4fd10)

2018/06/17
* メモしてなかったので、記憶が曖昧
* 建物、森、公園を書き出し出来るように変更
* 名前を「OSM Access Map」から「まち歩きマップメーカー」へ変更

2018/08/25
* PNG/SVGダウンロード時にCopyrightを追記するように(tom-kondaさんに感謝！)
* 信号のサイズを若干小さくする
* 「program by K.Sakanoshita」を削除

2019/01/03
* インターフェイスの見直し（画面を広く、画面遷移を分かりやすく）
* マップデータのダウンロード速度を改善（並列処理化）
* ダウンロード可能なファイルサイズを増加（古いブラウザだと重い）
* 恐らくInternetExploer11だと正常に動作しなくなったと思われます

2019/02/21 
* カフェのアイコンを表示・削除する機能を追加

2019/06/08
* レストラン、ファストフード、消火器、消火栓、避難所アイコンを表示する機能を追加
* 追加したアイコンに店舗名を表示するよう仕様変更（非表示やアイコン変更は今後）
* 追加したアイコンをドラッグアンドドロップで任意の場所へ移動する機能を追加
* 地図のデザインを見直し（色パレット追加、初期値の色を変更、線の太さなど）
* ユーザーインターフェースの見直し（表示/非表示のチェックボックスを統合など）

2019/08/09
* 更新情報を更新するのを忘れてました
* 地図スタイルを見直しました（少しGoogle Maps風？）
* カフェ以外にも消火器/避難所アイコンを追加出来ます
* その他にも、色々あるけど忘れました（笑）

2020/01/05
* 指定した年月日のデータをもとに描画する機能を追加
* 図書館、壁、ロープ、フェンス、擁壁を表示する機能を追加
* turf.jsの導入によるgeojsonのsimplifyを実施

2020/01/09
* ベンチを表示する機能を追加

2020/02/10
* 色選択を改善（クリックしやすく、選択状態を可視化）
* 選択出来る色数を増やしつつ、不要な色は削減
* 上記の機能強化に合わせて、標準地図の表現を見直す

2020/05/31
* 背景地図を openstreetmap.org から Maptiler へ変更
* 住所検索機能を追加(geoloniaの宮内氏に感謝！)
* 上記に合わせて画面レイアウトを一部変更（内部も見直し予定）
* ホスト先を netfort から GitHub へ変更

2020/07/06
* 「指定した年月日のデータを元に描画する機能」を一旦削除
* * かなり範囲を絞らないとサーバー側から応答が帰らないため
* 「turf.jsの導入によるgeojsonのsimplifyを実施」を削除
* * 大量のgeojsonを扱うことが目的で導入するも効果が低いため
