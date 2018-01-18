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
