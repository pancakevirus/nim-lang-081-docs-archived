---
layout: page
title: よくある質問と回答
css_class: faq
---

<h1 class="text-centered page-title main-heading">よくある質問と回答</h1>

# 一般的な質問

## 第三のプログラミング言語が必要な理由は？

Nim は数少ない「プログラム可能」な静的型付け言語であり、
C の速度とメモリの効率性、表情力豊かなシンタックス、
メモリの安全性と複数のターゲット言語を兼ね備えています。

## Nim は安定していますか？

コンパイラと標準ライブラリは積極的に開発が続けられており、
継続的な安定性を保証するためにテストケース一式を用意しております。
安定した基盤を求めているプロジェクト向けに基準として使用できる正規リリースを３～６ヶ月ごとに公開しております。
稀に破壊的変更が行われることはありますが、詳細情報は[ドキュメント化](https://nim-lang.org/blog/2018/03/01/version-0180-released.html)されているため、
通常は最小限の労力で対応可能であります。
また、コンパイラは必要十分な通知と移行期間を提供するために
廃止予定機能の強調表示を行います。


## セキュリティとメモリの安全性は？

Nim はポインター演算の実行不可、オプションの[チェック](https://nim-lang.org/docs/manual.html#pragmas-compilation-option-pragmas)、
参照のトレースとアントレース、さらにオプションの null 不可型によりメモリの安全性を提供しております。
これは koch ツールと汚染分析により Valgrind をサポートしております。

## Nim のライセンスは？

Nim のコンパイラとライブラリは MIT ライセンスです。
つまり、 Nim を用いて開発したプログラムには、
お好きなライセンスを適用できます。

## JVM/CLR バックエンドのサポート状況は？

最近の計画に JVM/CLR のサポートはありません。しかし、前述の仮想マシンは C の FFI をサポートしております。
よって Nim の強力なメタプログラミング機能を使い、透過的なグルーコード全体の生成を行うことでネイティブ Nim ブリッジの開発は可能であります。

## エディタのサポート状況は？

- Aporia (ネイティブ Nim エディタ): [https://github.com/nim-lang/Aporia](https://github.com/nim-lang/Aporia)
- Visual Studio Code: [https://marketplace.visualstudio.com/items?itemName=kosz78.nim](https://marketplace.visualstudio.com/items?itemName=kosz78.nim)
- Emacs: [https://github.com/nim-lang/nim-mode](https://github.com/nim-lang/nim-mode)
- Vim: [https://github.com/zah/nimrod.vim/](https://github.com/zah/nimrod.vim)
- QtCreator (4.1+): 実験的なプラグインとして収録済み。
- Scite: 収録済み
- Gedit: [Aporia の .lang ファイル](https://github.com/nim-lang/Aporia/blob/master/share/gtksourceview-2.0/language-specs/nim.lang)
- Geany: 収録済み
- jEdit: [https://github.com/exhu/nimrod-misc/tree/master/jedit](https://github.com/exhu/nimrod-misc/tree/master/jedit)
- TextMate: [https://github.com/textmate/nim.tmbundle](https://github.com/textmate/nim.tmbundle)
- Sublime Text: [https://github.com/Varriount/NimLime](https://github.com/Varriount/NimLime)
- LiClipse: [http://www.liclipse.com/](http://www.liclipse.com/) (Eclipse ベースのプラグイン)
- Howl: 収録済み
- Notepad++: [https://github.com/jangko/nppnim/releases](https://github.com/jangko/nppnim/releases)
- Micro: 収録済み
- Atom: [https://atom.io/packages/nim](https://atom.io/packages/nim)

## 言語設計で大いに影響を受けたものは？

大量に模倣した言語 (影響を受けた順) :
Modula 3, Delphi, Ada, C++, Python, Lisp, Oberon

## ``proc`` と命名した理由は？

*Procedure* (手続き) が一般用語として用いられるのとは対照的に *function* (関数)
は副作用のない数学的存在であります。実際のところ、 Nim の ``func`` は
``proc {.noSideEffect.}`` の糖衣構文です。 ``def`` は ``define`` (定義) の略記ですが、 
Nim では ``iterator`` (反復)と ``method`` (方法) キーワードを提供しているため ``def``
という命名では何を指しているのか意味が通じません。


# コンパイル関連の質問

## 最速動作の実行可能ファイルを生成するオプションは？

標準的な環境設定ファイルでは、 ``-d:release`` が秘訣です。
コンパイラでサポートしている場合は、リンク時の最適化を有効にすると
実行可能ファイルの動作速度をもっと向上できます: ``--passc:-flto``

## 最小容量の実行可能ファイルを生成するオプションは？

標準的な環境設定ファイルでは、 ``-d:quick --opt:size`` が秘訣です。
コンパイラでサポートしている場合は、リンク時の最適化を有効にすると
実行可能ファイルの容量をもっと縮小できます: ``--passc:-flto``

## デフォルトの C コンパイラとは違うものを使うには？

``config/nim.cfg`` ファイルを編集します。
変数 ``cc`` の値を下記の中から一つ選んで変更してください:

| 略称             | C/C++ コンパイラ                            |
| ---------------- | --------------------------------------------|
|``vcc``           | Microsoft Visual C++                        |
|``gcc``           | GNU C コンパイラ                            |
|``llvm_gcc``      | LLVM-GCC コンパイラ                         |
|``icc``           | Intel C コンパイラ                          |
|``clang``         | Clang コンパイラ                            |
|``ucc``           | 一般的な UNIX C コンパイラ                  |


それ以外の C コンパイラは公式にはサポートしておりませんが、動作する可能性があります。

上記のリストに記載されていない C コンパイラの場合は、 *一般的な UNIX C コンパイラ* (``ucc``)
を試してみてください。また、 C コンパイラで異なるコマンドライン引数が必要ならば
``--passc`` と ``--passl`` スイッチを試してみてください。
