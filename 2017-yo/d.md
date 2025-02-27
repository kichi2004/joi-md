配点： $100$ 点

### 問題
ある JOI 関係者は，おもちゃ屋で働いている．今日は，店内にあるぬいぐるみコーナーの整理をすることになった．

ぬいぐるみコーナーの棚には，$N$ 個のぬいぐるみが左から右に一列に並べられている．棚は仕切りにより $N$ 個の区画に区切られており，$1$ つの区画に $1$ 個のぬいぐるみを置く．このおもちゃ屋は合計 $M$ 種類のぬいぐるみを売っており，それぞれ $1$ から $M$ までの番号が付けられている．棚に並べられた $N$ 個のぬいぐるみは，それぞれこの $M$ 種類のうちのいずれかである．また，それぞれの種類のぬいぐるみは，少なくとも $1$ 個は存在する．

見栄えを良くするため，同じ種類のぬいぐるみが全て連続して棚に置かれるように，ぬいぐるみを並べ替えたい．次のような方法で，ぬいぐるみを並べ替えることにした．

- $N$ 個のぬいぐるみのうちいくつかを選び，棚から取り出す．取り出さなかったぬいぐるみの位置は動かさない．
- 取り出したぬいぐるみを，好きな順に棚の空いている区画に戻していく．

並べ替えた後，同じ種類のぬいぐるみが全て連続して棚に置かれていなければならない． 並べ替えるために取り出すぬいぐるみの個数の最小値を求めるプログラムを作成せよ．

---

### 入力
入力は $1 + N$ 行からなる．

$1$ 行目には $2$ 個の整数 $N, M$ ($1 \leqq N \leqq 100\,000$，$1 \leqq M \leqq 20$) が空白を区切りとして書かれており，ぬいぐるみが $N$ 個あり，種類が $M$ 種類あることを表す．

続く $N$ 行のそれぞれには，$1$ 以上 $M$ 以下の整数が書かれている．$N$ 行のうちの $i$ 行目 ($1 \leqq i \leqq N$) に書かれた整数は，棚の左から $i$ 番目の区画に置かれたぬいぐるみの種類を表す．各種類について，少なくとも $1$ 個のぬいぐるみが存在していることが保証される．

### 出力
並べ替えるために取り出すぬいぐるみの個数の最小値を $1$ 行で出力せよ．

---

### 入力例 1
```
7 2
1
2
2
2
1
2
1
```

### 出力例 1
```
2
```

入力例 $1$ においては，最初に置かれているぬいぐるみの種類は左から順に $1， 2， 2， 2， 1， 2， 1$ である．並べ替えるために取り出すぬいぐるみの個数を最小にするには，左から $1$ 番目と $6$ 番目のぬいぐるみを取り出し，左から $1$ 番目に種類 $2$ のぬいぐるみを，左から $6$ 番目に種類 $1$ のぬいぐるみを配置すればよい．このとき，取り出すぬいぐるみの個数は $2$ 個である．

---

### 入力例 2
```
12 4
1
3
2
4
2
1
2
3
1
1
3
4
```

### 出力例 2 
```
7
```

---
