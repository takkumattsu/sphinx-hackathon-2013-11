==============================
Sphinx ハッカソン 11/23
==============================

開催情報
============
1. 日時: 2013/06/30 13:00 - 12:00
2. 場所: 曙橋
3. 参加者: uasturn, tk0miya, koshw_nuts, masori335


Sphinxをはじめよう本
==========================

`ここから <http://www.oreilly.co.jp/books/9784873116488/>`_ 買おう！


今日の目標
============

**Jenkinsを利用してSphinxでドキュメント管理のノウハウをまとめる**

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

リンクの使い方
====================

1. 参照タイプのリンク
   
   1.1 Sphinx-user.jp_

       ``Sphinx-user.jp_ が呼ぶ方``

       ``.. _Sphinx-user.jp: http://sphinx-users.jp/  が定義``

2. 項目に対するリンク
   
   2.1. `Sphinxをはじめよう本`_

        ```Sphinxをはじめよう本`_``

3. 名前をつけてリンク
   
   3.1. 名前あり参照 `Sphinxjp <http://sphinx-users.jp/>`_
        
        ```Sphinxjp <http://sphinx-users.jp/>`_``

   3.2. 名前なし参照 `Sphinxjp <http://www.google.com>`__

        アンダースコアを二つをつけると無名参照になる(重複がオッケー)

        ```Sphinxjp <http://www.google.com>`__```

4. 直接URLをリンク
   
   4.1. http://sphinx-users.jp/

.. _Sphinx-user.jp: http://sphinx-users.jp/

スタイルについて
===================

tk0miyaさんはbizstyleを利用しているとのこと

.. code-block:: bash

   easy_install sphinxjp.themes.bizstyle

**1.2にはデフォルトで入るかもとのこと！**


PDF変換について
=================

Tex Live2013をインストールするとのこと

(ただし2.2GBあるので時間がかかるので注意、展開したあとも4GB食うとのこと)

* Windows, Linux系は Tex Live2013のインストールを行う

* Macの場合はMacTexというのをインストールする

  (homebrewだと古いのか、手動でインストールするように誘導される)


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
