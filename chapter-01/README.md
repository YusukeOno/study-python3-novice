# 予備知識

## 前段

- Pythonはインタプリタ型言語
- Pythonはオブジェクト指向言語
- Pythonはスクリプト言語
  - インデントによってブロックを表すので、正しくインデントを行わないとエラーになる
  - 半角4つで1段階のインデントを表すことを推奨されている
  - タブとインデントを混在させると意図しない動作になる
  - バージョン2と3は互換性があると言えない

## Pythonはインタラクティブモードで実行できる

ターミナルなどで、Pythonコマンドを引数なしで実行すると、インタラクティブモードで起動する。プロンプトは「>>>」が表示される。

終了するには、`exit()`コマンドを実行する

## 簡単な計算をする

```python
> python
Python 3.10.11 (main, Apr 15 2023, 12:23:53) [Clang 14.0.3 (clang-1403.0.22.14.1)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 1 +3
4
>>> 9-6
3
>>> exit()
```

## 演算の優先順位

他言語と同様

## 引数を表示するprint()関数

```python
> python
Python 3.10.11 (main, Apr 15 2023, 12:23:53) [Clang 14.0.3 (clang-1403.0.22.14.1)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> print(2024)
2024
>>> exit
Use exit() or Ctrl-D (i.e. EOF) to exit
>>> 
```

## 文字列はダブルクォーテーションで囲む

- 文字列の連結は「+」演算子を用いる
- 数値と文字列では型が異なる

数値と文字列を「＋」演算子で連結すると「TypeError」が発生する。

```python
>>> print(2024 + "年")
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: unsupported operand type(s) for +: 'int' and 'str'
```

- 数値を文字列に変換する`str()`関数

```python
>>> print(str(2024) + "年")
2024年
```
