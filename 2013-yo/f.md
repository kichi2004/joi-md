配点： $100$ 点

### 問題
オーストラリアに旅行に来た JOI 君は様々な場所で観光を楽しみ，ついに帰国する日がやってきた．今，JOI 君は帰りの飛行機が出発する国際空港のある町にいる．この町は東西南北に区画整理されており，各区画には道，土産店，住宅，国際空港がある． JOI 君は最も北西の区画から出発して最も南東の区画の国際空港を目指す．

JOI 君は今いる区画から隣り合った区画に移動することができるが，住宅のある区画には入ることはできない．また飛行機の時間に間に合わせるために，今いる区画の東か南の区画にのみ移動する．ただし，時間にはいくらか余裕があるため，$K$ 回まで今いる区画の北か西の区画へ移動することができる．

JOI 君は土産店のある区画に入ると，日本の友人たちのためにお土産を買う．JOI 君は土産店について入念に下調べをしていたので，どの土産店に行ったら何個のお土産を買うことができるかが分かっている．JOI 君が購入できるお土産の個数の最大値を求めるプログラムを作成せよ．

ただし，お土産を買う時間は無視できるとし，同じ土産店に $2$ 度以上訪れたときは最初に訪れたときだけお土産を買う．

---

### 入力
入力は $1 + H$ 行からなる．

$1$ 行目には，$3$ つの整数 $H, W, K$ ($2 \leqq H \leqq 50$，$2 \leqq W \leqq 50, 1 \leqq K \leqq 3$) が空白を区切りとして書かれている．

続く $H$ 行にはそれぞれ $W$ 文字からなる文字列が書かれており，区画の情報を表す．北から $i$ 番目，西から $j$ 番目の区画を $(i, j)$ と表す ($1 \leqq i \leqq H$，$1 \leqq j \leqq W$) ．$i$ 行目の $j$ 番目の文字は，区画 ($i, j$) が道か国際空港である場合は `.` であり，住宅である場合は `#` である． 土産店である場合は `1`，`2`，$\ldots$，`9` のいずれかであり，その土産店で買うことができるお土産の個数を表す．

与えられる入力データにおいては，JOI 君がはじめにいる最も北西の区画が道であることは保証されている．また，JOI 君が国際空港にたどり着けることは保証されている．

### 出力
JOI 君が購入できるお土産の個数の最大値を表す整数を $1$ 行で出力せよ．

---

### 入力例 1
~~~
5 4 2
...#
.#.#
.#73
8##.
....
~~~

### 出力例 1
~~~
11
~~~

入出力例 $1$ において，JOI 君は $3$ 回南へ進み区画 $(4, 1)$ の土産店で買い物をした後，さらに南へ $1$ 回，東へ $3$ 回進み，そこから北へ $2$ 回進むことで区画 $(3, 4)$ の土産店で買い物をする．最後に南へ $2$ 回進んで国際空港へたどり着くと，合計で $11$ 個のお土産を買うことができる．

---

### 入力例 2
~~~
4 4 3
.8#9
9.#.
.#9.
....
~~~

### 出力例 2
~~~
27
~~~
