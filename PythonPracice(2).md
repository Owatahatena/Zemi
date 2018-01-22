# 第二回
この章では制御構文について学びます。またプログラムの処理の流れや予約語やインデントについて学んでいきます。

## print

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

# 制御構文

## if文　条件分岐
条件に応じてやりたいことを決めるときに使う。
例えば`name`が田中太郎だったときとか`num`が10のときにとか…  

```python:if.py
num = 10
if num == 10:
    print(num)

if num > 10:
    print(num)

if num < 10:
    print(num)
```

## for文　繰り返し  
処理を繰り返すときに使う。  

```python:for.py
for i in range(10):
    print(i)
```

出力を確かめてみましょう。10回繰り返されていることがわかると思います。  
さて、ここでfor文の文法について解説しときたいと思います。
文法は`for i in range(num):`です。詳しく見てみましょう。
まずは`i`です。これはカウンタ変数と言って繰り返しの回数を数える変数になります。  
つぎに`range()`です。この関数は引数としてinteger型の数値を入れると0からその数-1まで繰り返すことができます。  
ほかにも

```python:f.py
for i in range(10):
    print(i) #0から9まで

for i in range(1,10):
    print(i) #1から9まで
```

このような使い方ができます。  


### イテレータ―について
pythonではforループを回す際に以下のような書き方もできます。

```python:ite.py
colords = ['red','blue','pink',green]

for color in colors:
    print(color)
```
結果を確認してみましょう。リストである`colors`の要素順々に取れたと思います。  
このようにリストをfor文に渡すと次の要素に次々とアクセスすることができます。このように次の要素に次々とアクセスすることができるインターフェースをイテレータと呼びます。  
