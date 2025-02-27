配点： $100$ 点

### 問題
JOI 君の住む IOI 市は，南北方向に $H$ 区画，東西方向に $W$ 区画の長方形の形をしており，$H \times W$ 個の区画に区切られている．北から $i$ 番目，西から $j$ 番目の区画を $(i, j)$ と表す．現在，IOI 市で開催されている国際的なプログラミングコンテストを記念して，大規模なお祭りが開催されている．いくつかの区画には屋台が出ており，それぞれ違う種類のお菓子を販売している． 区画 $(1, 1)$，区画 $(H, W)$ およびそれらに東西南北に隣接する区画には屋台はない．

JOI 君は区画 $(1, 1)$ から区画 $(H, W)$ に移動する．移動時間を短くするため，JOI 君は東あるいは南のみに移動を行う．JOI 君はお菓子が好きなので，区画に入るごとに順に次の行動をとる．

- 現在の区画にまだ買っていないお菓子を販売している屋台が出ている場合，その屋台でお菓子を購入する．
- 現在の区画の東西南北に隣接する区画にまだ買っていないお菓子を販売している屋台が出ている場合，それらの屋台のうち $1$ つを除く全ての屋台から販売員を呼んで，お菓子を購入する．

JOI 君は同じ種類のお菓子を複数回購入することはない．

IOI 市の大きさ，屋台の位置と，それぞれの屋台のお菓子の値段が与えられたとき，JOI 君が区画 $(1, 1)$ から区画 $(H, W)$ に移動する間に購入するお菓子の総額の最小値を求めよ．

---

### 入力
入力は $1 + H$ 行からなる．

$1$ 行目には，$2$ つの整数 $H, W$ ($3 \leqq H \leqq 1\,000$，$3 \leqq W \leqq 1\,000$) が空白を区切りとして書かれている．これは，IOI 市が $H \times W$ 個の区画に区切られていることを表す．

続く $H$ 行にはそれぞれ $W$ 文字からなる文字列が書かれており，IOI 市のそれぞれの区画の情報を表す．$H$ 行のうちの $i$ 行目の左から $j$ 番目の文字 ($1 \leqq i \leqq H$，$1 \leqq j \leqq W$) は，区画 $(i, j)$ に屋台がない場合には `.` （ピリオド）である．屋台がある場合には `1`, `2`, $\ldots$, `9` のいずれかであり，その屋台で販売しているお菓子の値段を表す．

与えられる $5$ つの入力データのうち，入力 $1$ では，屋台のある区画の数は $20$ 以下である．

### 出力
JOI 君が区画 $(1, 1)$ から区画 $(H, W)$ に移動する間に購入するお菓子の総額の最小値を $1$ 行で出力せよ．

---

### 入力例 1
~~~
5 5
..483
.59.9
3.866
79...
4.8..
~~~

### 出力例 1
~~~
20
~~~

入出力例 $1$ においては，区画 $(1, 1)$，区画 $(2, 1)$，区画 $(3, 1)$，区画 $(3, 2)$，区画 $(4, 2)$，区画 $(4, 3)$，区画 $(4, 4)$，区画 $(4, 5)$，区画 $(5, 5)$ の順番に移動して，区画 $(3, 1)$，区画 $(3, 3)$，区画 $(4, 2)$ の屋台で販売しているお菓子を購入すると，購入するお菓子の総額が最小となる．

---

### 入力例 2
~~~
12 10
..498522.4
.633527629
54.4621596
634.213458
1924518685
7739539767
276155.3.6
87716372.2
.858877595
7998739511
3438.5852.
568.9319..
~~~

### 出力例 2
~~~
63
~~~
