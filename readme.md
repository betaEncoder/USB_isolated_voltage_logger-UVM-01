# USB isolated voltage logger UVM-01
-USB絶縁電圧計-

![image](image.jpg)

# これは何？
測定した電圧を Tera Term 等のターミナルソフトウェアに表示するモジュールです．

PCと測定対象の間は絶縁されているため，電位差やグラウンドループなどを気にせず測定することができます．

![terminal](terminal.png)

鉛フリー，RoHS対応部品を使用しています．

# 仕様
## シリアルポート
- 115200 baud
- パリティ無し
- フロー制御無し
## 測定仕様
- 測定対象：直流電圧
- サンプルレート：最大1000サンプル/秒
- 測定レンジ切り替え：自動/固定
- 測定レンジ：L(0-3V)，H(0-30V)

| Range | L | H |
| ----|----|----|
| 分解能 | 1mV | 10mV |
| 入力抵抗 | 10MΩ | 1MΩ |

# コマンド
コマンドにより設定を変更することができます．

| コマンド | 設定内容 | 引数 |
|----|----|----|
| interval | 測定周期 | 0～10000（ms単位で指定） |
| range | 測定レンジを指定 | auto(自動切替)/L/H |
| autostart | 接続後自動測定を開始する | on/off |
| start | 自動測定がoffの場合に測定を開始する |  |
| unit | 単位(V)を表示する | on/off |
| help | コマンド一覧を表示 |  |

# 基板サイズ(図面)
簡易的な図面と3Dモデルを用意しました．PDFと3Dモデル(STEP/PARASOLID)がダウンロード可能です．

このデータは寸法を保証するものではありません．参考値としてご利用ください．

- [PDF](Assembly_Drawings.PDF)
- [STEP](UVM-01.step)
- [PARASOLID](UVM-01.x_t)
