

ライセンス
--------
Nim のライセンスに準ずるものとします。ただし、翻訳物にも著作権があります。
また、主要翻訳者は一切の対価を得ていません。個人・法人などを問わず書面による
事前許諾なしに商用利用、および就職・転職活動などにおいて、経歴詐称など不正利用は固く禁じます。

商業利用の場合は、必ず事前に許諾を得てください。
その場合のプロジェクト支援の対価は任意であり強制ではありません。許諾だけでも励みになります。


作業記録
--------
対象バージョン : Nim 1.0.6
作業対象ファイル : 完了: 51 - 合計 : 181 = 残り : 130

Jan : 31
Feb : 29 (Current: 19 / 10)  → 60
Mar : 31 (Current:  0 / 31)  → 91
Apr : 

Feb の目標 : 80 ～ 120 (前半～中盤)

仮訳完了:
	asyncfile.html
	asynchttpserver.html
	base64.html
	browsers.html
	cookies.html
	cpuinfo.html
	cpuload.html
	distros.html
	docgen_sample.html
	dom.html
	endians.html
	highlite.html
	htmlgen.html
	iup.html
	jsconsole.html
	jscore.html
	koch.html
	linenoise.html
	md5.html
	mersenne.html
	mimetypes.html
	mysql.html
	nimgrep.html
	nimprof.html
	nimtracker.html
	odbcsql.html
	oswalkdir.html
	overview.html
	packaging.html
	punycode.html
	registry.html
	segfaults.html
	sha1.html
	sharedlist.html
	sqlite3.html
	sugar.html
	termios.html
	theindex.html
	time_t.html
	tools.html
	util.html
	varints.html
	volatile.html
	widestrs.html
	winlean.html
	wordwrap.html
	xmlparser.html
	codeowners.html
	htmlparser.html
	dynlib.html
	chains.html


翻訳活動への参加方法
--------------------
1. 事前にツール (OSDN, OmegaT, TMX/TBX Editor, Git など) の使いかたを理解してくださるようお願いします。

* OmegaT (4.3.1 以降。ただし安定版のみ)                 : https://www.omegat.org/
* Okapi Framework (6.038 以降)                          : https://okapiframework.org/
* Rogrus Global Goldpan TBX/TMX Editor (3.3 以降)       : https://logrusglobal.com/goldpan.html
* WinMerge                                              : https://winmerge.org/
* BusyBox                                               : https://www.busybox.net/
* TortoiseGit                                           : https://tortoisegit.org/
* Xbench                                                : https://www.xbench.net/
* Anchovy                                               : https://www.maxprograms.com/products/anchovy.html



辞書の指定は後ほど。


翻訳活動への参加方法 (注意点)
-----------------------------

内輪揉めをしているほど人生は暇ではありません。利用者の混乱を避けるため、フォークの乱立は避けてください。

* 主要翻訳者、および関係者へメールで送られても対応できません。
* Google翻訳などウェブ翻訳サービスを使用した訳出結果のコミットはライセンス規約上の問題以外にも、
  ニューラル翻訳特有の問題があります。正確さを保証・検証できないため使用を禁止させていただいております。


対応可能ファイル形式
--------------------


推奨形式:
* OmegaT プロジェクト
* TSV (UTF-8 エンコーディング)
* tmx


対応可能形式:
* FUJITSU ATLUS 翻訳 2004 以降
* LogoVista コリャ英和！  一発翻訳 2009 以降
* TOSHBA The翻訳 V10 以降

それ以外につきましてはご相談ください。


寄贈者
------
・主要翻訳者: isVowel (Twitter: @isvowel)


----------------------------------------------------------------------------------------------------
付録 (後で別ファイルへ分離します)
----------------------------------------------------------------------------------------------------


プロジェクトが読み込めない (OmegaT)
-----------------------------------
「プロローグにはコンテンツを指定できません」エラーが表示されている場合は omegat.project が壊れています。
Git リポジトリからコピーしなおしてください。これはノートパソコンなど電源の不安定に成りやすい環境で稀に起きるようです。


LogoVista コリャ英和！  一発翻訳形式 (krydoc)
---------------------------------------------
この形式は機械翻訳版であり品質は保証できません。
アライメントの調整など修正などは順次行いますが、作業優先順位は低いです。

閲覧と編集には「LogoVista コリャ英和！  一発翻訳 2020」以降が必要です。
捨て値で手に入りやすい「LogoVista コリャ英和！  一発翻訳 2009 」以降での編集はできますが、
環境によってロックされた文節を編集しようとすると落ちたり、ツールバーが吹っ飛んだりするバグが潜んでいますので
お勧めしません。

この形式のファイルは下記フォルダに収録してあります。

* nim/docs/LogoVista/*

注意: 
  主要翻訳者によるコリャ英和の使用は Nim を以て終了となるため、
  この形式の提供は OmegaT 版の全仮訳完了後に受付・更新終了となります (Nim 1.0.8 ～ 1.0.10 公開後の予定)。

備考: krydoc 形式の実態は zip ファイルです。
      SrcText (原文), TrgText (訳文) からテキストファイルを取り出すことができます。
      よって、翻訳エディタとテキストエディタで修正後に busybox (paste コマンド)、アライメントツールなどを使って
      tmx へ変換することは可能です 。


LogoVista コリャ英和！  一発翻訳 (雑記)
---------------------------------------
krydoc → tmx ファイルへの変換方法については、こちらがお勧めです。
翻訳エディタを疑似アライメントエディタとして使うことができますし、完全オフラインでの作業ができます。

参考ファイル
* nim/docs/LogoVista/tmx

前提条件
 - ApSIC Xbench 2.9 以降 
    v.2.9 はフリーソフトウェア、それ以降は商用ソフトです。

 - Goldpan TBX/TMX Editor 3.3 以降

作業の流れ
 - 1. コリャ英和！  一発翻訳 2020
   - アライメントの調整と機械翻訳（ポストエディット）
   - TSVファイルの作成 : ファイル(F) → テキストの書き出し(E) → 左右対訳(B)...

 - 2. TSVファイルの修正、または編集
   - テキストエディタ、 あるいは Microsoft Office, LibreOffice Calc などの表計算ソフトでも編集可能です。
   - ほかのファイルとのマージなどもできます。

 - 3. ApSIC Xbench で TSV → tmx へ変換
      Okapi Framework での変換もできるようです。

 - 4. Goldpan TBX/TMX Editor で修正・編集
 - 5. OmegaT の tm フォルダへコピー。

※この方法であれば、ほかの機械翻訳ソフトと OmegaT を併用できるかと思います。

※いまのところ、コリャ英和シリーズには TSV, CSV ファイルのインポート機能がないので
   手軽に (tmx → krydoc) へ戻す方法はありません。  gawk で TSV ファイルのフィールドを切り出して
   SrcText と TrgText を krydoc ファイルへ圧縮し直す方法も考えられますが、動作保証はありません (おそらく不明な翻訳エンジンエラーになると思います)。


LogoVista コリャ英和！  一発翻訳 2020 - 翻訳の不具合
------------------------------------------------------------
Twitter (@isvowel) でも書いていますが...。
このソフトはバグが...。

- apis.html
	should return an int with the < 0 == 0 or > 0 semantics; for a bool result use sameXYZ
	→翻訳できず原文が返されるだけでなく、グループ指定ができなくなる。他社製ソフトなら問題ない。

- for : 辞書の問題で、for の訳文が誤訳である「賛成の」になってしまう (おまけに、訳出禁止にできない)。

- iterator : 辞書によっては「アイテレータ」と誤訳されてしまう。


LogoVista コリャ英和！  一発翻訳 2020 - ファイル翻訳の不具合
------------------------------------------------------------
下記のファイル (Nim 1.0.6 - 調査中) を翻訳するとハングアップ (または「不明な翻訳エンジンエラー」) になる場合があります。
- dom.html
- iup.html
- manual.html
- mysql.html
- net.html
- openssl.html
- os.html
- pcre.html
- posix.html
- postgres.html
- sqlite3.html
- system.html
- tables.html
- termios.html
- theindex.html
- times.html
- winlean.html

解決策として、

・これらのファイルはウェブブラウザから開き、ページ全体をコピー、その後に翻訳エディタへ張り付けて下さい。
・また、翻訳エディタで直接読み込み (レイアウトビューモードで)。

なお、 manual.htmlは処理に時間がかかりますので、テキストを分割して処理することをお勧めします。

誤って処理対象としてしまった場合はタスクマネージャーを起動して

・ファイル翻訳 (32ビット)
・E to J 翻訳エンジン エンジンモジュール (32ビット)
・翻訳エンジン ロケータモジュール (32ビット)

の順に強制終了してください。または、 taskkillコマンドでも構いません。

taskkill /F /IM K21Grinder.exe
taskkill /F /IM K21EJTranslationEngine.exe
taskkill /F /IM K21TranslationEngineLocator.exe

そのあとに異常動作を起こすときは、コリャ英和関連のアプリを全て終了し %temp% フォルダを開いてテンポラリファイルをすべて削除してください。

また、翻訳エディタとファイル翻訳の併用は避けてください（環境によっては併用すると動作不良の原因となります）。

