![fo200_1](iamges/fo200_1)
- Start列から001行にある０を抜いた数字を抜き出す（今回は32768）
- フラグファイルがないか探す
```bash
sudo fls -o 32768 -r diskimage.raw.001 | head -n 50 | grep flag
```
```
結果
+++ r/r 69-128-1:       flag.rar
```
```bash
sudo icat -o 32768 diskimage.raw.001 69 > flag.rar
```
```bash
cat flag.rar
```
※開封注意
・flag.larの内容を確認（pngファイル発見）
