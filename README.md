# jelly_soup

# Usage
指定したプルダウンリスト（option valueとタグ間の文字列）をコマンドラインで表示します。動的に生成されるリストにはまだ未対応です。
また、表示したoption valueとタグ間の文字列はエクセルにタイムスタンプ付きファイル名で保存します。
```
opt_list_{%y%m%d_%H%M%S}.xlsx
```

# Example

```
python yumyum_jelly_soup.py https://yumyumjelly.github.io/index.html .select-list
```

**sample html**

```html
<ol class="select-list">
  <li>
    <select id="cate_a" name="cate_a">
      <option value="">1. category A</option>
      <option value="1" title="aaa">aaa</option>
      <option value="2" title="bbb">bbb</option>
      <option value="3" title="ccc">ccc</option>
      <option value="4" title="ddd">ddd</option>
      <option value="5" title="eee">eee</option>
    </select>
  </li>
</ol>
```

**sample result (.xlsx)**
| column A (value) | column B (string)      |
|:-----------------|:-----------------------|
|                  |1. category A           |
|1                 | aaa                    |
|2                 | bbb                    |
|3                 | ccc                    |
|4                 | ddd                    |
|5                 | eee                    |
