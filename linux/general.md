# Linuxとは
OSの一種。<br>
Unixをまねて開発された。<br>
コードが無料で公開されており、さまざまな形式で配布されている。

# カーネル
Linuxの根幹となるコンポーネント。狭義のLinux。<br>
機能として、ハードウェア制御、ソフトウェアの実行などを持つ。<br>
一般的を可能にするために、カーネルに機能を付け加えてさまざまな形式のLinuxが配布されている。

# ディストリビューション
Linuxカーネルにさまざまな機能を付け加えて作成されたLinux。一般的に指すLinux。<br>
大きくRedHat系、Debian系、Slackware系のベースがある。

## RedHat系
- **Red Hat Enterprise Linux(RHEL)**<br>
有料でリリースされている。<br>
サポートが充実している。<br>
RedHat系のディストリビューションの多くはRHELのソースコードから派生している。

- **Cent OS**<br>
無償利用。<br>
RHELのクローンとして作成された。<br>
個人利用に向いている。

- **Fedora**<br>
無償利用。<br>
RHELの検証としての役割を持つ。<br>
安定性は低いが、最新技術が早くに導入されている。

## Debian系
- **Debian GNU/Linux**<br>
無償利用。<br>
世界中の有志の技術者によって開発されている。<br>
Debian系ディストリビューションの多くに派生している。

- **Ubuntu**<br>
無償利用。<br>
誰にでも使いやすいように作成された。

# シェル
Linuxコマンドをコンピュータに渡すソフトウェア。<br>
実行結果の画面表示も担当する。
コマンドの入力/出力にはターミナル、コマンドプロンプトといったソフトウェアが担当する。

- **sh**<br>
最も基本的なシェル。<br>
多くの派生が存在する。

- **bash**<br>
shから派生。<br>
shに機能を追加した上位互換。

- **zsh**<br>
さらに多くの機能を追加したシェル。<br>
別系統のcsh、tcshの機能までのほぼ網羅している

## 現在使用しているシェルを確認する
```terminal
echo $SHELL
```










