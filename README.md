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
  - [大文字か小文字か判定](#%E5%A4%A7%E6%96%87%E5%AD%97%E3%81%8B%E5%B0%8F%E6%96%87%E5%AD%97%E3%81%8B%E5%88%A4%E5%AE%9A)
- [数値](#%E6%95%B0%E5%80%A4)
  - [平方数](#%E5%B9%B3%E6%96%B9%E6%95%B0)
- [list](#list)
  - [ソート](#%E3%82%BD%E3%83%BC%E3%83%88)
    - [昇順・降順](#%E6%98%87%E9%A0%86%E3%83%BB%E9%99%8D%E9%A0%86)
    - [逆順](#%E9%80%86%E9%A0%86)
- [数値](#%E6%95%B0%E5%80%A4-1)
  - [平方数](#%E5%B9%B3%E6%96%B9%E6%95%B0-1)
- [文法](#%E6%96%87%E6%B3%95)
    - [range](#range)

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
```

## 複数行

### 1列


だいたい1行目の入力として行数(n)が提供される。

```
s_list = [input() for i in range(n)]
i_list  = [int(input()) for v in range(n)]

# 行数指定がない場合はtry-exceptを使う
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

## 大文字か小文字か判定

```
s.isupper()
s.islower()
```

# 数値

## 平方数

```
sn = sr ** 0.5
sn = pow(sr, 0.5)
```

# list

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

# 数値

## 平方数

```
sqr = sqn ** 0.5
sqr = pow(sqn, 0.5)
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
