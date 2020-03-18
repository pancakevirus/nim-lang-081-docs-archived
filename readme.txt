
ライセンス
--------
Nim のライセンスに準ずるものとします。ただし、翻訳物にも著作権があります。
また、主要翻訳者は一切の対価を得ていません。

個人・法人などを問わず書面による商業利用の場合は、必ず事前に許諾を得てください。
その場合のプロジェクト支援の対価は任意であり強制ではありません。許諾だけでも励みになります。

また、就職・転職活動などにおいて、経歴詐称など不正や盗用行為は固く禁じます
もちろん、寄贈者が記載していいのは、あなたが担当した部分だけです。


作業記録
--------
対象バージョン   : Nim 1.0.6
作業対象ファイル : 完了: 78 ( +10 = krydoc) - 合計 : 181 = 残り : 102 ( 93 = accounts krydoc)

・序盤戦終了 : 2020/02/27 (Done: 60) Jan ～ Feb 期間
・序盤戦開始 : 2020/02/28 Mar ～ Apr 期間

^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Jan : 31 (Current: 31 / 31)  →  31 - 181 = 150 : Achieved!!!
Feb : 29 (Current: 29 / 29)  →  60 - 181 = 121 : Achieved!!!
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Mar : 31 (Current: 18 ( +10 = krydoc) / 31)  →  91 - 181 =  90
Apr : 30 (Current:  0 / 30)  → 121 - 181 =  60
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
May : 31 (Current:  0 / 31)  → 151 - 181 =  30
Jun : 30 (Current:  0 / 30)  → 180 - 181 =   1
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Jul : 10
Aug : 10
Sep : 10
Oct : 10
Nov : 10
Dec : 10


予測
--------
Nim 1.0.8 公開 : 2020/03/28


仮訳完了:
	assertions.html
	asyncfile.html
	asyncftpclient.html
	asynchttpserver.html
	base64.html
	browsers.html
	chains.html
	codeowners.html
	colors.html
	complex.html
	cookies.html
	cpuinfo.html
	cpuload.html
	distros.html
	docgen_sample.html
	dom.html
	dynlib.html
	editdistance.html
	encodings.html
	endians.html
	highlite.html
	htmlgen.html
	htmlparser.html
	io.html
	iup.html
	jsconsole.html
	jscore.html
	koch.html
	linenoise.html
	locks.html
	marshal.html
	md5.html
	mersenne.html
	mimetypes.html
	mysql.html
	nimgrep.html
	nimprof.html
	nimtracker.html
	odbcsql.html
	oids.html
	ospaths.html
	oswalkdir.html
	overview.html
	packaging.html
	parsesql.html
	punycode.html
	rdstdin.html
	registry.html
	rlocks.html
	rst.html
	rstast.html
	rtarrays.html
	segfaults.html
	sha1.html
	sharedlist.html
	sqlite3.html
	sugar.html
	termios.html
	theindex.html
	time_t.html
	tools.html
	typetraits.html
	unidecode.html
	util.html
	varints.html
	volatile.html
	widestrs.html
	winlean.html
	wordwrap.html
	xmlparser.html
	xmltree.html
	smtp.html
	openssl.html
	nimscript.html
	sums.html
	lexbase.html
	dollars.html
	diff.html
	(J) critbits.krydoc         / .txt : tmx 変換待ち
	(J) cstrutils.krydoc        / .txt : tmx 変換待ち
	(J) cgi-000.krydoc          / .txt : tmx 変換待ち
	(J) asyncstreams-000.krydoc / .txt : tmx 変換待ち
	(J) estp-000.krydoc         / .txt : tmx 変換待ち
	(J) threads-000.krydoc      / .txt : tmx 変換待ち
	(J) niminst-000.krydoc      / .txt : tmx 変換待ち
	(J) apis-000.krydoc         / .txt : tmx 変換待ち
	(J) tinyc-000.krydoc        / .txt : tmx 変換待ち
	(J) channels-000.krydoc     / .txt : tmx 変換待ち


翻訳活動への参加方法
--------------------
事前にツール (OSDN, OmegaT, TMX/TBX Editor, Git など) の使いかたを理解してくださるようお願いします。
これらは、すべてフリーソフトウェア (寄付歓迎、開発協力歓迎も対象) です。

* OmegaT (4.3.0 以降。ただし安定版のみ)                 : https://www.omegat.org/
* Okapi Framework (6.038 以降)                          : https://okapiframework.org/
* Rogrus Global Goldpan TBX/TMX Editor (3.3 以降)       : https://logrusglobal.com/goldpan.html
* WinMerge                                              : https://winmerge.org/
* BusyBox                                               : https://www.busybox.net/
* TortoiseGit                                           : https://tortoisegit.org/
* Xbench                                                : https://www.xbench.net/
* Anchovy                                               : https://www.maxprograms.com/products/anchovy.html
* Stanford Log-linear Part-Of-Speech Tagger             : https://nlp.stanford.edu/software/tagger.shtml

・OmegaT はメインの翻訳環境として使います。TMXが扱えるなら、ほかのCATツール (例えばBasicCAT) でも構いません。
・Okapi Framework は翻訳メモリの各種処理に使います。
  例えば翻訳メモリに対応していない機械翻訳ソフトの対訳データを TMX へ変換することもできます。
・Goldpan TBX/TMX は翻訳メモリデータベースの編集に使います。OmegaT などの翻訳メモリは定期的に保守整備を行わないと訳出精度が落ちるため、このようなソフトでの編集が必要です。
・Xbench は翻訳メモリのフォーマット変換、翻訳品質検査などに使います。
・Anchovy は Maxprograms Swordfish にバンドルされているフリーソフトウェアの用語集データベースエディタです。
・Part-Of-Speech Tagger は英文の品詞解析に使います。
・WinMerge は新旧バージョンの比較と変更箇所の検出に使います。

・パソコンのメモリは最低でも 8GB (Windows機) ほど必要です。 OmegaT だけで 1.2GB ほど消費します。
  VisualStudio などと併用しながら...となると 4GB では、かなりきついです。


共通辞書の指定
--------------
こればかりは、フリーソフトウェアで良いものがないので、きちんと正規品を購入してください。

・英辞郎 第11版 (辞書データVer.159 / 2020年1月8日版) 以降
  https://ec.alc.co.jp/book/7020008/

注意点: PDIC-R形式ですので、ほかのソフトでの串刺し検索はできません (変換方法は公開されておりません)。
EBWin4/EBPocket などで、ほかの辞書との串刺し検索をしたい方は、
書籍第8版ではなく、きちんと修正が施された EDPのサイトより旧版 (Ver.144.8)をお求めください。

その他に英米俗語辞典 (引用句の翻訳) や英和学習辞典が必要です (手持ちのものをお使いください)。

それ以外にもOALD9など置いておきたいものはありますが、あまり無理は言えません。


引用句について
--------------------
国内では愛好家以外なじみのない洋楽、洋物ゲームに関する知識が必要です。
スラングがわからないと訳せないものもあります。

・ラムシュタイン
・System Shock2

など。他言語の訳者もうまく訳せていないかたを多く見かけます (2020年現在、ニューラル翻訳でも正確な翻訳は不可能です)。
自信がなければ、そのままにしておいたほうが良いでしょう。


機械翻訳ソフトの指定
--------------------
あれば便利ですが、買わなくていいです。
LogoVista コリャ！英和 本格翻訳 2020 を使っていますが、翻訳作業に不慣れなかた向けに使っている面が強いです。

日本全国どこでも手に入りやすく、個人経営の書店でも注文できることくらいですかね。
ただ。今後、使用を終了する方針で作業を進めています。やはり、バグに泣かされることが多いんで。
これを書いていた数時間前も三十分ほどかけた原稿が印刷プレビューのバグで飛んでしまい、本当に捨てたくなりました。


翻訳活動への参加時にかかる必要
------------------------------
追加初期機材費用として 5000～10000 円以内とします (主に辞書代です)。
機械翻訳ソフトウェアは任意です (みんなの自動翻訳が使えるかは未だ検討中)。
用意しなくても、いずれ翻訳メモリデータベースが蓄積されていきますので次第にいらなくなるでしょう。
そしてChromebook (Linux対応機) でも作業ができるようなると思います。

国内の Nim のユーザー層であると考えられる「平均的な学生さん/月平均のお小遣い2500～円」で
捻出できる範囲を想定しております。

活動参加のための飲食代、宿泊費、通信費、電気代などは算入していません。



翻訳活動への参加方法 (注意点)
-----------------------------
内輪揉めをしているほど人生は暇ではありません。利用者の混乱を避けるため、フォークの乱立は避けてください。

* 主要翻訳者、および関係者へメールで送られても対応できません。かならず OSDN のリポジトリへプルリクエストしてください。
* Google翻訳などウェブ翻訳サービスを使用した訳出結果のコミットはライセンス規約上の問題以外にも、
  ニューラル翻訳特有の問題があります。正確さを保証・検証できないため使用を禁止させていただいております。


対応可能ファイル形式
--------------------

推奨形式:
* OmegaT プロジェクト
* TSV (UTF-8 エンコーディング)
* tmx
* XLIFF

対応可能形式 (2020年03月現在):
* Microsoft Excel / Word
* Libre Office
* FUJITSU ATLUS 翻訳 2004 以降
* LogoVista コリャ英和！  一発翻訳 2009 以降
* TOSHBA The翻訳 V10 以降

それ以外につきましてはご相談ください。


寄贈者
------
・主要翻訳者: isVowel (Twitter: @isvowel)


担当(記載例)
・hogefile.html - foobar さん (連絡先/URL)
・品質管理 (用語集データベース)     : foobar  さん (連絡先/URL)
・品質管理 (翻訳メモリデータベース) : foobar2 さん (連絡先/URL)


