---
layout: page
title: Unix 版のインストール
css_class: install_unix
current: Install
---

<h1 class="text-centered page-title main-heading">Nim のインストール (Unix 版)</h1>

# ``choosenim`` によるインストール

[``choosenim``](https://github.com/dom96/choosenim#choosenim) は
プログラミング言語 Nim のインストーラーです。最新の安定版リリース、
または最新の開発版との間で Nim 
バージョンの切り換えを簡単にできるようにします。

``choosenim`` で Nim の最新の安定版リリースをインストールするには、
下記のコマンドをターミナルで実行してから、画面の指示に従ってください:

```bash
curl https://nim-lang.org/choosenim/init.sh -sSf | sh
```

# 手動インストール

## ビルド済みバイナリ (Linux 版)

<div class="center">
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}-linux_x32.tar.xz"
    class="pure-button pure-button-primary download-button">
    <i class="fa fa-file-archive-o" aria-hidden="true"></i>
    x86版の入手 (tarball形式)
  </a>
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}-linux_x32.tar.xz.sha256"
    class="pure-button">
    <i class="fa fa-file-text-o" aria-hidden="true"></i>
    SHA256
  </a>
</div>

<div class="center">
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}-linux_x64.tar.xz"
    class="pure-button pure-button-primary download-button">
    <i class="fa fa-file-archive-o" aria-hidden="true"></i>
    x86_64版の入手 (tarball形式)
  </a>
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}-linux_x64.tar.xz.sha256"
    class="pure-button">
    <i class="fa fa-file-text-o" aria-hidden="true"></i>
    SHA256
  </a>
</div>

## ソースアーカイブ

<div class="center">
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}.tar.xz"
    class="pure-button pure-button-primary download-button">
    <i class="fa fa-file-archive-o" aria-hidden="true"></i>
    ソース版の入手 (tarball形式)
  </a>
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}.tar.xz.sha256"
    class="pure-button">
    <i class="fa fa-file-text-o" aria-hidden="true"></i>
    SHA256
  </a>
</div>

圧縮形式のアーカイブをダウンロードし終えたら、
ご希望のインストールディレクトリへアーカイブの内容を展開します。
ビルド済みバイナリはバイナリ・ディストリビューション (配布形態) で提供されています。

ソース・ディストリビューションでは、新しいターミナルのウィンドウを開き、
``cd`` で展開先のディレクトリへ移動し、下記の手順に従ってコマンドを実行します:

```bash
sh build.sh
bin/nim c koch
./koch tools
```

## 手動インストールにおける環境変数 ``PATH`` の設定

さて、コンパイラとツールのバイナリは ``bin`` ディレクトリにあります。
一般に Nim 開発者は[環境変数 ``PATH``](https://en.wikipedia.org/wiki/PATH_(variable))
へ下記のディレクトリを指定してパスを通します:

* 前述の ``bin`` ディレクトリ
* ``~/.nimble/bin`` (``~`` はホームディレクトリ)

# バイナリのインストールに関する注意点

Nim コンパイラはソフトウェアのコンパイルをするために C コンパイラが必要です。別途、
コンパイラのインストールを行い、必ず ``PATH``を通してください。


## macOS

システムで利用可能な clang の最新版をインストールするだけです。
この手順に従います:

* 新しい「ターミナル」のウィンドウを開きます。
* ``xcode-select --install`` を実行します。
* ダイアログボックスの表示後に "Install" ボタンをクリックします。

**出典:** [Quora](https://www.quora.com/How-do-I-successfully-set-up-LLVM-clang-on-Mac-OS-X-El-Capitan/answer/James-McInnes-1?srid=hq2O)

## Linux

おそらく、コンパイラはインストールは済みです。そうでなければ、
パッケージマネージャーで ``gcc`` または ``clang`` をインストールしてください。

# そのほかの依存性

Nim を使うために依存性のインストールが必要になる場合があります。
対象は:

* PCRE
* OpenSSL

上記の依存性が必要な時は、
パッケージマネージャーでインストールできます。

# パッケージマネージャーによるインストール

## Arch Linux

```
pacman -S nim
```

## Debian / Ubuntu

```
apt-get install nim
```

## Docker

コミュニティにより保守管理されている [Docker イメージ](https://hub.docker.com/r/nimlang/nim/)は
Docker Hub で配布されています。
イメージにはコンパイラと Nimble を収録してあります。
Nimble パッケージと同じように、スタンドアローン・スクリプト用のイメージがあります。

安定版のイメージを取得するには:

```
docker pull nimlang/nim
```

最新開発版のイメージを取得するには:

```
docker pull nimlang/nim:devel
```

## Fedora

```
dnf install nim
```

## FreeBSD

```
pkg install nim
```

## macOS

```
brew install nim
```

## openSUSE

```
zypper in nim
```

## Snap

```
snap install nim-lang
```

## Void Linux

```
xbps-install -S nim
```
