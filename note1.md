# MNE Python チュートリアル

## 1章 入門チュートリアル

### 1,MNE-PythonによるMEG/EEG解析の概要

#### データの読み込み
MNE-Pythonはさまざまなデータ形式に対応できる。対応するデータ形式を以下に示す。

- .edf, .bdf, .gdf (European Data Format)
- .cnt (Neuroscan CNT format)
- .fif (Elekta Neuromag FIF format)
- .brainvision (BrainVision format)

※ 本チュートリアルでは、FIFファイルを用いている。

MEG/EEG解析は、まずデータを読み込むことから始める。
データの読み込みは<u>tutorial1.ipynb</u>のプログラム1にて行われる。
**mne.datasets.sample.data_path()関数**は、サンプルデータセットのローカルコピーへのパスを取得できる。
想定される場所のいずれにもデータセットが見つからない場合、自動的にデータセットをダウンロードし、データセットへのディレクトリパスを返します。
**mne.io.read_raw_fif()関数**は、生のFIFデータを読み取る機能を持つ。
これによりデータの読み取り、および情報を取得できる。

また、より詳しい情報を取得する場合は、<u>tutorial1.ipynb</u>のプログラム2にて取得できる。
これは、データを読み取ったrawをプリントすることで取得している
.infoに関しては、<u>note1.md</u>の4,Infoデータ構造にて説明する。

rawオブジェクトには、さまざまなプロット形式がある。
ここでは、<u>tutorial1.ipynb</u>のプログラム3にて示した2つの関数を説明する
**raw.compute_psd()関数**は、センサーデータに対してスペクトル解析を実行する関数である。
**raw.plot()関数**は、生データをプロットする関数である。

#### 前処理




### 2,データの変換



### 3,生データからイベントを解析



### 4,Infoデータ構造



### 5,センサー位置の操作



### 6,MNE-Pythonの設定



### 7,mne.reportの利用開始