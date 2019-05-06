procon-cheatsheet
---

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [標準入力](#%E6%A8%99%E6%BA%96%E5%85%A5%E5%8A%9B)
  - [1行](#1%E8%A1%8C)
    - [1列](#1%E5%88%97)
    - [複数列](#%E8%A4%87%E6%95%B0%E5%88%97)
  - [複数行](#%E8%A4%87%E6%95%B0%E8%A1%8C)
    - [1列](#1%E5%88%97-1)
    - [複数列](#%E8%A4%87%E6%95%B0%E5%88%97-1)
- [文字列](#%E6%96%87%E5%AD%97%E5%88%97)
  - [大文字、小文字の操作](#%E5%A4%A7%E6%96%87%E5%AD%97%E5%B0%8F%E6%96%87%E5%AD%97%E3%81%AE%E6%93%8D%E4%BD%9C)
    - [大文字か小文字か判定](#%E5%A4%A7%E6%96%87%E5%AD%97%E3%81%8B%E5%B0%8F%E6%96%87%E5%AD%97%E3%81%8B%E5%88%A4%E5%AE%9A)
    - [先頭を大文字、それ以降を小文字にする](#%E5%85%88%E9%A0%AD%E3%82%92%E5%A4%A7%E6%96%87%E5%AD%97%E3%81%9D%E3%82%8C%E4%BB%A5%E9%99%8D%E3%82%92%E5%B0%8F%E6%96%87%E5%AD%97%E3%81%AB%E3%81%99%E3%82%8B)
  - [ゼロ埋め](#%E3%82%BC%E3%83%AD%E5%9F%8B%E3%82%81)
- [数値](#%E6%95%B0%E5%80%A4)
  - [平方数](#%E5%B9%B3%E6%96%B9%E6%95%B0)
  - [ある数が2べきかどうかの判定](#%E3%81%82%E3%82%8B%E6%95%B0%E3%81%8C2%E3%81%B9%E3%81%8D%E3%81%8B%E3%81%A9%E3%81%86%E3%81%8B%E3%81%AE%E5%88%A4%E5%AE%9A)
  - [円周率](#%E5%86%86%E5%91%A8%E7%8E%87)
  - [ビット演算](#%E3%83%93%E3%83%83%E3%83%88%E6%BC%94%E7%AE%97)
    - [AND演算](#and%E6%BC%94%E7%AE%97)
    - [OR演算](#or%E6%BC%94%E7%AE%97)
    - [XOR演算](#xor%E6%BC%94%E7%AE%97)
    - [ビット反転(-(a+1)する)](#%E3%83%93%E3%83%83%E3%83%88%E5%8F%8D%E8%BB%A2-a1%E3%81%99%E3%82%8B)
    - [左シフト(ビットを左にずらす)](#%E5%B7%A6%E3%82%B7%E3%83%95%E3%83%88%E3%83%93%E3%83%83%E3%83%88%E3%82%92%E5%B7%A6%E3%81%AB%E3%81%9A%E3%82%89%E3%81%99)
    - [右シフト(ビットを右にずらす)](#%E5%8F%B3%E3%82%B7%E3%83%95%E3%83%88%E3%83%93%E3%83%83%E3%83%88%E3%82%92%E5%8F%B3%E3%81%AB%E3%81%9A%E3%82%89%E3%81%99)
- [配列(list)](#%E9%85%8D%E5%88%97list)
  - [検索](#%E6%A4%9C%E7%B4%A2)
    - [値からインデックス](#%E5%80%A4%E3%81%8B%E3%82%89%E3%82%A4%E3%83%B3%E3%83%87%E3%83%83%E3%82%AF%E3%82%B9)
  - [ソート](#%E3%82%BD%E3%83%BC%E3%83%88)
    - [昇順・降順](#%E6%98%87%E9%A0%86%E3%83%BB%E9%99%8D%E9%A0%86)
    - [逆順](#%E9%80%86%E9%A0%86)
- [辞書(dict)](#%E8%BE%9E%E6%9B%B8dict)
  - [ループ](#%E3%83%AB%E3%83%BC%E3%83%97)
    - [キーだけ使う](#%E3%82%AD%E3%83%BC%E3%81%A0%E3%81%91%E4%BD%BF%E3%81%86)
    - [値だけ使う](#%E5%80%A4%E3%81%A0%E3%81%91%E4%BD%BF%E3%81%86)
    - [キーと値の両方を使う](#%E3%82%AD%E3%83%BC%E3%81%A8%E5%80%A4%E3%81%AE%E4%B8%A1%E6%96%B9%E3%82%92%E4%BD%BF%E3%81%86)
- [集合(set)](#%E9%9B%86%E5%90%88set)
- [文法](#%E6%96%87%E6%B3%95)
    - [range](#range)
- [集合演算](#%E9%9B%86%E5%90%88%E6%BC%94%E7%AE%97)
  - [和集合(OR)](#%E5%92%8C%E9%9B%86%E5%90%88or)
  - [積集合(AND)](#%E7%A9%8D%E9%9B%86%E5%90%88and)
- [数え上げ](#%E6%95%B0%E3%81%88%E4%B8%8A%E3%81%92)
  - [Counter](#counter)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# 標準入力

## 1行

### 1列

```
s = input()
s = int(input())
```

### 複数列

```
m, n = input().split()
m, n = map(int, input().split())

# 配列として
m_list = list(map(int, input().split()))

# タプルとして
m_list = tuple(map(int, input().split()))

# 別パターン
m_list = [i for i in input().split()]
```

## 複数行

### 1列


だいたい1行目の入力として行数(n)が提供される。

```
s_list = [input() for i in range(n)]
i_list  = [int(input()) for v in range(n)]
```

行数指定がない場合はtry-exceptを使う。

```
while True:
    try:
        a_list = list(map(int, input().split()))
    except:
        break
```

### 複数列

```
# 文字列として
s_list = [input().split() for i in range(n)]

# 数値として
s_list = [map(int, input().split()) for i in range(n)]
```

# 文字列

## 大文字、小文字の操作

参考: https://note.nkmk.me/python-capitalize-lower-upper-title/

### 大文字か小文字か判定

```
s.isupper()
s.islower()
```

### 先頭を大文字、それ以降を小文字にする

```
str = 'atcoder'
str.capitalize() # 'Atcoder'
```

## ゼロ埋め

formatメソッドを使う方法。
ex. 2ケタ0埋め

```
h=n//3600
m=(n-3600*h)//60
s=n-(3600*h+60*m)
print('{:02}:{:02}:{:02}'.format(h, m, s))
```

# 数値

## 平方数

```
sn = sr ** 0.5
sn = pow(sr, 0.5)
```

## ある数が2べきかどうかの判定

nとn-1とのAND演算の結果が0なら2べき。

```
if not n & n - 1:
  print('power of 2')
```

## 円周率

mathモジュールを使う。

```
import math

pi = math.pi
```

## ビット演算

- 参考
  - https://www.javadrive.jp/python/num/index4.html 
  - https://www.javadrive.jp/python/num/index5.html

```
a=11 # 0b1011
b=14 # 0b1110
```

### AND演算

```
a&b # 10(1010)
```

### OR演算

```
a|b # 15(1111)
```

### XOR演算

```
a^b # 5(0101)
```

### ビット反転(-(a+1)する)

```
~a # -12(-1100)
```

### 左シフト(ビットを左にずらす)

```
a<<1 #22(10110)
```

### 右シフト(ビットを右にずらす)

```
b>>1 #7(111)
```

# 配列(list)

## 検索

### 値からインデックス

indexメソッドを使う。最初に当てはまったインデックスだけを返す。

```
abc_list = ['a', 'b', 'b', 'c']
print(abc_list.index('b')) #-> 1
```

## ソート

### 昇順・降順

ソートされた新しいリストを作る。

```
sorted(arr)

# 降順
sorted(arr, reverse=True)
```

既に存在するリストをソートする。

```
arr.sort()

# 降順
arr.sort(reverse=True)
```

### 逆順

順番を入れ替える。

```
sample_list = sample_list[::-1]
```

# 辞書(dict)

## ループ

### キーだけ使う

```
abc_dict = {'a': 0, 'b': 1, 'c': 2}
for k in abc_dict.keys():
    print(k)
```

### 値だけ使う

```
abc_dict = {'a': 0, 'b': 1, 'c': 2}
for v in abc_dict.values():
    print(v)
```

### キーと値の両方を使う

```
abc_dict = {'a': 0, 'b': 1, 'c': 2}
for k, v in abc_dict.items():
    print(k, v)
```



# 集合(set)

重複のない配列みたいなやつ。

```
initial_set = set()

# 要素の追加
set.add('a')

# 要素の削除
set.remove('a')

# 全要素の削除
set.clear()
```

# 文法

### range

https://docs.python.org/ja/3/library/stdtypes.html#range

range(start, stop[, step])
stopの値になったら停止するので、forループ内に出てくる値はstart以上stop未満。

```
for i in range(1, 5):
    print(i)
     
# output
1
2
3
4
```

# 集合演算

## 和集合(OR)

いずれかのグループに含まれる値をリストアップする。

```
s_union = s1 | s2
s1.union(s2)
```

## 積集合(AND)

いずれのグループにも含まれる値をリストアップする。

```
s_intersection = s1 & s2
s1.intersection(s2)
```

# 数え上げ

## Counter

指定した文字列、配列内の要素を数え上げる。

```
from collections import Counter

s = 'abcabcabcd'
s_cntr = Counter(s) #-> Counter({'a': 3, 'b': 3, 'c': 3, 'd': 1})
type(s_cntr)        #-> <class 'collections.Counter'>
dict(s_cntr)        #-> {'a': 3, 'b': 3, 'c': 3, 'd': 1}
```
