---
layout: page
title: Windows 版のインストール
css_class: install_windows
current: Install
---


<h1 class="text-centered page-title main-heading">Nim のインストール (Windows 版)</h1>

<div class="center">
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}_x32.zip"
    class="pure-button pure-button-primary download-button">
    <i class="fa fa-file-archive-o" aria-hidden="true"></i>
    x86版の入手 (zip形式)
  </a>
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}_x32.zip.sha256"
    class="pure-button">
    <i class="fa fa-file-text-o" aria-hidden="true"></i>
    SHA256
  </a>
</div>

<div class="center">
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}_x64.zip"
    class="pure-button pure-button-primary download-button">
    <i class="fa fa-file-archive-o" aria-hidden="true"></i><!-- 「～版のダウンロード (zip 形式)」にするとレイアウトが崩れてしまう。 -->
    x86_64版の入手 (zip形式)
  </a>
  <a href="{{ site.baseurl }}/download/nim-{{ site.nim_version }}_x64.zip.sha256"
    class="pure-button">
    <i class="fa fa-file-text-o" aria-hidden="true"></i>
    SHA256
  </a>
</div>

# バイナリのインストールに関する注意点

提供されている zip ファイルでのインストールは、かなり簡単です。
ご希望のインストールディレクトリへファイルを展開してから
``finish.exe`` を実行します (場合により管理者権限での実行が必要です)。

## 環境変数 ``PATH`` の設定

さて、バイナリは zip ファイルから ``bin`` ディレクトリにあります。
一般に Nim 開発者は[環境変数 ``PATH``](https://en.wikipedia.org/wiki/PATH_(variable))
へ下記のディレクトリを指定してパスを通します:

* 前述の ``bin`` ディレクトリ
* ``%USERPROFILE%\.nimble\bin`` (``%USERPROFILE%`` はホームディレクトリ)

簡単に bin ディレクトリへの ``PATH`` を追加するアプリケーションとして
``finish.exe`` を zip ファイルに収録してあります。
また、このツールは C コンパイラの有無を確認します。無ければ Windows 版
GNU C コンパイラ・コレクションである ``MinGW`` をインストールすることもできます。

# コンパイラの依存性に関する注意点

Nim コンパイラはソフトウェアのコンパイルをするために C コンパイラが必要です。
``finish.exe`` で ``MinGW`` をインストールできます。

このバージョンの ``MinGW`` は、最新版の Nim
で動作確認済みです。

<!-- TODO: Instructions on what to do with these 7z files? -->

* 32 bit - [mingw32.7z]({{ site.baseurl }}/download/mingw32.7z)
* 64 bit - [mingw64.z]({{ site.baseurl }}/download/mingw64.7z)

# そのほかの依存性

Nim を使うために依存性のインストールが必要になる場合があります。
対象は:


* PCRE
* OpenSSL

Windows ユーザは、[こちらから]({{ site.baseurl }}/download/dlls.zip)
共有ライブラリ (DLL) をダウンロードできます。ダウンロードした共有ライブラリは
`nim.exe` と同じディレクトリに配置してください。
