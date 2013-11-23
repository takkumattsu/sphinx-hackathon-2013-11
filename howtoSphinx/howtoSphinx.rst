リンクの使い方
====================

1. 参照タイプのリンク
   
   1.1 Sphinx-user.jp_

       ``Sphinx-user.jp_ が呼ぶ方``

       ``.. _Sphinx-user.jp: http://sphinx-users.jp/  が定義``

2. 項目に対するリンク
   
   2.1. `リンクの使い方`_

        ```リンクの使い方`_``

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

bloakdiagについて
===================

画面遷移図などをマークアップ形式でかける！
差分も分かりやすいし、図がずれることもないよ！

詳しくは以下
http://blockdiag.com/ja/blockdiag/

以前自分で入れるときにまとめたような
TODO

toctreeについて
=================

章ごとにディレクトリを切るいい感じみたい

.. blockdiag::

   blockdiag {
     // Set labels to nodes.
     A [label = "Topのindex.rst"];
     B [label = "大項目1"];
     C [label = "大項目2"];
     D [label = "中項目1"];
     E [label = "中項目2"];
     F [label = "小項目1"];
     G [label = "小項目2"];
     H [label = "小項目3"];
     I [label = "小項目4"];

     A -> B
     A -> C
     B -> D
     C -> E
     D -> F
     D -> G
     E -> H
     E -> I
   }


Sphinxのエラーチェック
======================

-W オプションをつければ-Werror相当のことができる

Makefileに

SPHINXOPT=-W

jenkins
==============

シェルスクリプトは普通のsphinxコマンドmake html

成果物保存に以下を指定
build/**

説明に最新成果物のリンクを貼ってあげる


