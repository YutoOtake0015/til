# 概要
Node.jsのバージョン管理ツール。

# 特徴
1. 動作が速い
2. プロジェクト単位でのバージョン変更が容易
3. OSを問わず使用可能(Linux, MacOS, Windows)
4. 複数のパッケージマネージャをサポート
5. アップグレード毎の再インストールが必要ない
などなど

# インストール
## MacOS
1. Homebrewでパッケージをインストールする。
```terminal
brew install volta
```
2. 以下コマンドでパスを追加する。
```terminal
volta setup
```
  
 - 初期化ファイル内にPathが追加される
   - Path
     - export VOLTA_HOME="$HOME/.volta"
     - export PATH="$VOLTA_HOME/bin:$PATH"
   - 初期化ファイル
     - .bash_profile
     - .bashrc
     - .zshrc
     - .config/fish/config.fish
     - .profile
