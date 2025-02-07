# コンテナ

## 準備

1. [Google Colaboratory](https://research.google.com/colaboratory/)で「Python 3の新しいノートブック」を作る．
1. ノートブックの名前を「05」に変える．

## 演習

**問題** メソッドの練習：`"Hello".upper()`の結果を確認せよ．

**問題** メソッドの練習：`"Hello".replace("l", "e")`の結果を確認せよ．

**問題（レポート課題）** 文字列が持つメソッドを使う例を5個作れ．ヒント：https://docs.python.org/ja/3/library/stdtypes.html#string-methods

**問題** 以下のコンテナについて，絵を描いて説明せよ．

* リスト
* タプル
* セット
* 辞書

タプルは**イミュータブル**（変更不可能），他は**ミュータブル**（変更可能）である．

**資料**

項目|リスト|タプル|セット|辞書
----|------|------|------|----
空のコンテナの作成|`list()`，`[]`|`tuple`，`()`|`set()`|`dic()`，`{}`
要素を含むコンテナの作成|`[要素, ...]`|`(要素, ...)`|`{要素, ...}`|`{キー:値, ...}`
要素の読み取り|`x[番号]`|`x[番号]`||`x[キー]`，`x.get(キー)`
要素の更新|`x[番号] = 値`|||`x[キー] = 値`
要素の追加|`x.append(値)`||`add(値)`|`x[キー] = 値`
要素の削除|`x.pop()`，`x.pop(番号)`||`x.remove(値)`|`x.pop(キー)`
要素の存在確認|`値 in x`|`値 in x`|`値 in x`|`キー in x`
要素数の取得|`len(x)`|`len(x)`|`len(x)`|`len(x)`
コンテナの連結|`x + y`|`x + y`|＊|

＊の部分は`x.union(y)`，`x.intersection(y)`，`x.difference(y)`

**問題** リストについて，以下の操作を行え．

```python
a = [10, 20, 30, 40]

# 「50」を末尾に追加

# 2番目を表示

# 1番目を200に変更

# 3番目を削除

# 要素数を表示

# すべて表示
```

**問題** セットについて，以下の操作を行え．

```python
b = {10, 20, 30, 40}

# 「50」を追加

# 「30」は入っているか？

# 「60」は入っているか

# 「20」を削除

# 要素数を表示

# すべて表示
```

**問題** 辞書について，以下の操作を行え．

```python
c = {'A':10, 'B':20, 'C':30}

# 「"D":50」というペアを追加

# "B"というキーは入っているか？

# "E"というキーは入っているか

# "A"というキーを削除

# 要素数を表示

# すべて表示
```

**問題** 郵便番号（7桁の数値，ハイフンなし）から住所を求められるようにするためには，どのようなコンテナを使えばよいか．

**問題** `[10, 20, 30, 20, 10, 10, 20]`というリストから重複を削除せよ．順番は保存しなくてよい．

**問題（レポート課題）** リスト・タプル・セット・辞書の違いを，コードを使って説明せよ．
