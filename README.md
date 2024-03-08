# CPUのシミュレーション
<br>

## 概要
論理回路シュミレータを用いたCPUの再現
<br><br>

## 開発の目的
CPUがどのように計算や情報を処理しているかを学習する
<br><br>

## 使用技術
Logisim（論理回路シュミレータ）<br> http://www.cburch.com/logisim/
<br><br>

## 閲覧方法
Logisimをダウンロードし、本リポジトリのファイルCPU.circをロードする
<br><br>

## 概要
- 論理回路を用いて、演算命令（足し算など）を与えて、指定した数同士の演算がどのように行われるかをシュミレートしました
- 演算に使いたい数字を格納するメモリ、CPU全体の動きを制御するコントローラ、演算器、命令デコーダーなどCPUに組み込まれているユニットの一つ一つを論理回路で作成し、統合してCPUにしました

## 作成したCPUとCPU各部の構成図（一部抜粋）
### メモリ

<br><br>

### ALU（Arithmetic and Logic Unit）
四則演算や論理演算を行うCPU内部の装置
- a、bは演算に使用する2つの数（足し算であれば足す2つの数）
- opは命令文、どの種類の演算（加算、比較など）かを選択し、対応する演算のユニットのみに信号を送る
<img width="848" alt="スクリーンショット 2024-03-08 16 57 33" src="https://github.com/null64-null/CPU-simulation/assets/127968084/836e7381-7268-4e6a-8057-108a24f36731">
<br><br>

### CPU
作成したすべてのユニットを統合して、実際のCPUを論理回路で再現
<img width="981" alt="スクリーンショット 2024-03-08 16 59 34" src="https://github.com/null64-null/CPU-simulation/assets/127968084/034c806e-4824-49b9-a3b6-4ed5a9377743">
<br><br>

## 今後やりたいことなど
論理回路で一からPCを作成するゲームを作ってみたいです。
<br><br>

## ライセンス
本リポジトリのライセンスは、 MIT ライセンスの規約に基づいて付与されています
（LICENCE に記載）
<br><br>

【参考書籍】
本シミュレーションは、以下の書籍を参考にしました
But How Do It Know? - The Basic Principles of Computers for Everyone  （J Clark Scott 著 ）