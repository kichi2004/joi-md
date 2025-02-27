配点： $100$ 点

### 問題
あなたはクリスマスパーティーに学校内の自分の友達と，自分の友達の友達を招待することにした．あなたの通う学校の生徒数は $n$ 人であり，それぞれの生徒には $1$ から $n$ までの番号が割り振られている．あなたの番号は $1$ である．あなたの手元には，誰と誰が友達であるかを記したリストがある．このリストをもとに，あなたがクリスマスパーティーに招待する生徒数を求めるプログラムを作成せよ．

---

### 入力
入力の $1$ 行目には学校の生徒数 $n$ ($2 \leqq n \leqq 500$) が，$2$ 行目にはリストの長さ $m$ ($1 \leqq m \leqq 10\,000$) が書かれている．入力は全部で $2 + m$ 行からなる．$2 + i$ 行目 ($1 \leqq i \leqq m$) には $2$ つの整数 $a_i$ と $b_i$ ($1 \leqq a_i < b_i \leqq n$) が空白区切りで書かれており，番号 $a_i$ と番号 $b_i$ の生徒が友達同士であることを表す．入力の $3$ 行目から $2 + m$ 行目には同じ友達関係を表す行が重複して現れることはない．

### 出力
出力は，あなたがクリスマスパーティーに招待する生徒数のみを含む $1$ 行からなる．

---

### 入力例 1
~~~
6
5
1 2
1 3
3 4
2 3
4 5
~~~

### 出力例 1
~~~
3
~~~

入力例 $1$ において，あなたの友達は番号 $2$ と番号 $3$ の生徒の $2$ 人である．また，番号 $3$ と番号 $4$ の生徒は友達同士であるので，番号 $4$ の生徒はあなたの友達の友達である．番号 $5$ と番号 $6$ の生徒はあなたの友達でもなく，あなたの友達の友達でもない．したがって，あなたは番号 $2, 3, 4$ の $3$ 人の生徒をクリスマスパーティーに招待する．

---

### 入力例 2
~~~
6
5
2 3
3 4
4 5
5 6
2 5
~~~

### 出力例 2
~~~
0
~~~

入力例 $2$ において，あなたには友達はいない．したがって，あなたがクリスマスパーティーに招待する生徒数は $0$ 人である．
