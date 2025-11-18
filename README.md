# N-net観測点データ (_非公式_)
防災科学技術研究所の南海トラフ海底地震津波観測網「N-net」の観測点のデータです。観測点の緯度・経度・深さに加え、気象庁の[コード表](https://xml.kishou.go.jp/tec_material.html)に記載のコード・観測点名などを含みます。
<img width="1431" height="765" alt="image" src="https://github.com/user-attachments/assets/a4ee58d2-842a-4652-8388-232fe9fabdae" />
Made with Natural Earth.

## データ内容
### 表1 keyと値の関係
|key|例|出典番号|説明|
|-|-|-|-|
|code_nied|N.NAE01|1|防災科研による「観測点コード」|
|code_jma|61071|4|コード表に記載の「Code」|
|name|高知沖６０ｋｍＢ|4|コード表に記載の「Name」|
|kana|こうちおき６０ｋｍＢ|4|コード表に記載の「ふりがな」|
|lat|32.7687|1|観測点の設置緯度（北緯;世界測地系）|
|lng|134.2661|1|観測点の設置経度（東経;世界測地系）|
|depth_m|1563|1|観測点の水深（m）|
### 配布データ
- nnet.csv
- nnet.json
- nnet.geojson

csv、json形式のデータは、各観測点について、表1に示す項目が記録されている。  
geojson形式のデータは、[JGD2011](https://epsg.io/6668)で作成され、各観測点がPoint地物で記録されている。また、各地物のpropertiesに表1に示す項目が記録されている。
空欄は無い。


## 作成手法
出典1から取得した観測点データよりGISデータを形成し、出典2・3を参考にGISソフトウェア上で出典4のコード表と突合した。作成後、全数検査を行った。

## 出典
1. [防災科研 海底地震津波観測網ウェブサイト 「観測点情報」](https://www.seafloor.bosai.go.jp/st_info/)
2. [気象庁 報道発表資料「津波情報等に活用する観測地点の追加について ～「南海トラフ海底地震津波観測網（N-net）」沿岸システムの活用開始～」](https://www.jma.go.jp/jma/press/2511/14b/20251114_N-net.html)
3. [気象庁 報道発表資料「津波情報等に活用する観測地点の追加について ～「南海トラフ海底地震津波観測網（N-net）」沖合システムの活用開始～」](https://www.jma.go.jp/jma/press/2411/14a/20241114_N-net.html)
4. [気象庁 個別コード表「地震火山関連コード表」](https://xml.kishou.go.jp/tec_material.html)
