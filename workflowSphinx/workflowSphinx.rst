WindowsでrestreucturedTextを使う
=================================

vimかemacs使えよ、以上

といいたいけど社内にはサクラエディタ勢がすごいいる...

なのでWindowsで動くrestructuredTextのシンタックス対応エディタ

さくらエディタの設定
 http://advent-calendar2012.usaturn.net/2012/12/03/writing_tool.html

 http://advent-calendar2012.usaturn.net/2012/12/10/make_on_sakura.html

SublimeText
 TODO

Sphinxの運用について
======================

実際に社内で利用しているtk0miyaさんに聞いてみました。

* Jenkinsの利用
* 出力フォーマット
    
  * PDF
  * HTML

流れ
------

1. push

2. jenkinsでビルド

3. 成果物としてHTMLとPDFを出す

4. すごい幸せ

PDF変換について
=================

Tex Live2013をインストールするとのこと

(ただし2.2GBあるので時間がかかるので注意、展開したあとも4GB食うとのこと)

* Windows, Linux系は Tex Live2013のインストールを行う

* Macの場合はMacTexというのをインストールする

.. list-table:: texのインストール
   :header-rows: 1


   * - OS
     - インストーラー
   * - Windows
     - http://www.tug.org/texlive/windows.html
   * - Linux系
     - ftp://ftp.riken.go.jp/pub/tex-archive/systems/texlive/Images/
   * - Mac
     - http://tug.org/mactex/
