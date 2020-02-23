# jelly_soup
指定のプルダウンリスト（option valueとタグ間の文字列）を表示します。動的に生成されるリストにはまだ未対応です。

表示したoption valueとタグ間の文字列はエクセルにタイムスタンプ付きファイル名

（opt_list_{%y%m%d_%H%M%S}.xlsx'）で保存します。

**e.g.,**

test_soup.py https://yumyumjelly.github.io/index.html .select-list
