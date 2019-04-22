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
