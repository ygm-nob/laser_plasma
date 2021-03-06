# laser_plasma
レーザー生成プラズマの実験、研究で使うスクリプト集\

# fft.py

スペース区切りの 2 列のデータ(1 列目が時間、2列目が信号強度)の FFT
データ(スペクトル強度 と位相)を求める python スクリプト．python は ver.3
を用いている．

## インストール方法

`phython3` は、`/usr/loca/bin/python3`
にインストールされているとしている．\
`> which python3`\
で示される `PATH` が 1
行目と一致していなければ、その出力に書き換える．`PATH`
の通ったところに保存し、\
`> chmod +x fft.py`\
で実行許可を与える．

実行時に、パッケージのインストールを要求されたら、\
`> pip3 install numpy`\
`> pip3 install argparse`\
で、インストールすること． numpy や argparse
は初期にはインストールされていない．\

## 使い方

`> fft.py -h`\
で簡単な使い方の help が表示される\
optional arguments:\
-h, --help, show this help message and exit\
-g, --gnuplot, gnuplot で作成したグラフ(pdf)を表示\
-c, --csv, csv file を指定(デフォルトは space 区切り)\
-s, --silent, -g
オプションを指定しているとき、グラフ(pdf)の画面表示をしない(eps
は保存されます)\
-n, --norm, 最大値で規格化(eps は保存されます)\
