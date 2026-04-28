## ■ マルウェア解析で使用したツール

### 🔹 Procmon（Process Monitor） – Microsoft公式
Windows のファイル/レジストリ/プロセス監視ツール。
- **詳細**: [Microsoft Learn - Procmon](https://learn.microsoft.com/sysinternals/downloads/procmon)

### 🔹 Wireshark – ネットワーク解析（通信IP取得）
ネットワークパケットをキャプチャする世界標準ツール。
- **詳細**: [Wireshark Official](https://www.wireshark.org/download.html)

### 🔹 Regshot – レジストリ比較ツール
実行前後のレジストリ差分を取るCTF定番ツール（CTF勢がよく使う安定版）。
- **SourceForge**: [Regshot Project](https://sourceforge.net/projects/regshot/)
- **GitHub ミラー (最新版)**: [Seabreg/Regshot](https://github.com/Seabreg/Regshot)

### 🔹 PECmd
Eric Zimmerman氏による、Windowsのプリフェッチ（Prefetch）ファイルを解析するための強力なコマンドラインツール。
- **詳細**: [Eric Zimmerman's Tools](https://ericzimmerman.github.io/#!index.md)

### 🔹（参考）Strings / Binwalk
Windows向けバイナリ解析で使う場面があるツール群。
- **GNU strings (Windows版)**: [Sysinternals Strings](https://learn.microsoft.com/sysinternals/downloads/strings)
- **Binwalk**: [ReFirmLabs/binwalk](https://github.com/ReFirmLabs/binwalk)
  - ※解析にはPython環境が必要。
