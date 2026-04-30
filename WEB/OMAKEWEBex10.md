## WEBEX10のおまけ

### インストールされていなかったコマンドがあったから、それをインストールしたんだけどおもったよりうまくいかなかったから一連の流れを記載

### gitコマンドをインストールしたい！！！から始まった長い闘い
```
┌──(kali㉿kali)-[~]
└─$ git clone https://github.com/arthaud/git-dumper.git
python3 git-dumper/git_dumper.py $URL/.git/ dumped_repo
cd dumped_repo
git log --oneline --all

Cloning into 'git-dumper'...
remote: Enumerating objects: 204, done.
remote: Counting objects: 100% (104/104), done.
remote: Compressing objects: 100% (46/46), done.
remote: Total 204 (delta 69), reused 60 (delta 58), pack-reused 100 (from 2)
Receiving objects: 100% (204/204), 66.14 KiB | 7.35 MiB/s, done.
Resolving deltas: 100% (106/106), done.
Traceback (most recent call last):
  File "/home/kali/git-dumper/git_dumper.py", line 17, in <module>
    import dulwich.index
ModuleNotFoundError: No module named 'dulwich'
cd: そのようなファイルやディレクトリはありません: dumped_repo
fatal: not a git repository (or any of the parent directories): .git
```
- すべてはこのエラーから始まった
  
### 要はコマンドのインストール手順（上から順に）

```bash
sudo apt update
sudo apt install -y python3-pip
```
```bash
sudo apt update
sudo apt install -y python3-dulwich
```
```bash
python3 -c "import dulwich, dulwich.index; print('dulwich OK', dulwich.__version__)"
```
```bash
sudo apt update                                                                     
sudo apt install -y python3-requests-pkcs12
```

```bash
sudo apt install -y python3-venv
```
```bash
python3 -m venv ~/venv-gitdumper
source ~/venv-gitdumper/bin/activate
```
```bash
pip install --upgrade pip
pip install dulwich requests-pkcs12
```
```bash
python3 git-dumper/git_dumper.py $URL/.git/ dumped_repo
```
```bash
pip install beautifulsoup4
```
```bash
python3 git-dumper/git_dumper.py $URL/.git/ dumped_repo
```
```bash
pip install pysocks
```
