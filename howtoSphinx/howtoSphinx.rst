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

