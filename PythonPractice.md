# Pythonの入門

## 変数について  
変数とは箱のようなもの。なんらかの値を格納する。  
静的な型システムのある言語では変数には決まった型があり1,23,100などでは整数型、1,233などは小数型となる。  

### 変数の宣言
プログラムの中で変数をどの名前でどの型なのかを明示すること。各プログラミング言語により文法は異なる。

```c:a.c
int integer_num; //Cでの整数型の宣言 この場合`integer_num`という名前で整数型の変数として扱うという意味
```

### 代入
宣言した変数に対しデータを結びつける操作のこと  

```c:a.c
int integer_num; //変数の宣言

integer_num = 10; //10という整数のデータをinterger_numのメモリ領域と結びつける
```


### pythonにおける変数
pythonでは変数に値が格納されるのではなくデータ(オブジェクト)に対して名前（変数名)をタグ付けするイメージ  
変数の宣言は必要ない  

```python:s.py
name = "Imamura"
```

### pythonでの代入
```python:d.py
num = 1111 #受ける側が左辺、入れたいものが右辺
```

## pythonのデータの型
さて、先ほどの変数の宣言の説明でデータには型があることは理解したとおもいます。そしてpythonの変数にはどんな型でも入れられるということも抑えれましたか？  
この項ではpythonで扱うデータの型の紹介をしたいと思います。  
pythonでデータの型を知るためには`type`を使います。では実際にデータの型を確認していきましょう。  

```python:t.py
name = 'imamura'
print(type(name))

>> <class 'str'>
```
`<class 'str'>`と出力されたと思います。classについてはとりあえず置いておいて（後ほど詳しく説明します）`str`というのがありますよね？
それがデータの型になります。str(string)つまり文字列型になります。  

ほかのデータでも試してみましょう。  

```python:t.py
num = 124
print(type(num))

>> <class 'int'>

```
```python:y.py
num = 1.234
print(type(num))

>> <class 'float'>

```

```python:t.py
l = []
print(type(l))

>> <class 'list'>

```

```python:t.py
d = {}
print(type(d))

>> <class 'dict'>
```



## print

基本構文①

```python:p.py
print("Hello, World")
```

`print()`は出力の組み込み関数である。  

用例：  
- 文字列の出力

```python:s.py
s = "Hello,World" #strオブジェクトにsという名前を付ける.
print(s) #出力
```  

- 数値の出力

```python:num.py
num = 100
print(num)

num = 1.111
print(num)
```
