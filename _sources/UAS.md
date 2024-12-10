### UAS
## Soal 1
| $NO$ | $P$ | $Q$ | $R$ | $S$ | $P \rightarrow Q$ | $R \rightarrow S$ | ($P \rightarrow Q$) $\rightarrow$ ($R \rightarrow S$) |
| ---- | --- | --- | --- | --- | --- | --- | --- |
| 1    | T   | F   | T   | F   |  F  |  F  |  T  |
| 2    | F   | T   | T   | T   |  F  |  T  |  F  |
| 3    | T   | F   | T   | T   |  F  |  T  |  F  |
| 4    | T   | F   | F   | F   |  F  |  T  |  F  |
| 5    | F   | F   | F   | F   |  T  |  T  |  T  |
| 6    | F   | T   | T   | F   |  F  |  F  |  T  |
| 7    | T   | T   | T   | T   |  T  |  T  |  T  |
| 8    | F   | F   | F   | T   |  T  |  F  |  F  |


## Soal 2

![graph uas](https://hackmd.io/_uploads/HJgoDf4E1g.png)

Hitung Closeness Centrality:



| Node | A   | B   | C   | D   | E   | F   | G   |
| ---- | --- | --- | --- | --- | --- | --- | --- |
| A    | 0   | 1   | 2   | 2   | 3   | 2   | 3   |
| B    | 1   | 0   | 1   | 1   | 2   | 1   | 2   |
| C    | 2   | 1   | 0   | 2   | 3   | 2   | 3   |
| D    | 2   | 1   | 2   | 0   | 1   | 2   | 2   |
| E    | 3   | 2   | 3   | 1   | 0   | 1   | 1   |
| F    | 2   | 1   | 2   | 2   | 1   | 0   | 1   |
| G    | 3   | 2   | 3   | 2   | 1   | 1   | 0   |

Jawab:
Cc(B) $\frac{7-1}{1+1+1+2+1+3}$= $\frac{6}{9}$= 0,6

Hitung Betweenness Centrality:

Node: B
| Node | $$\sigma_{uw}$$ | $$\sigma_{uw}(B)$$ | $$\frac{\sigma_{uw}(B)}{\sigma_{uw}}$$ |
| ---- | --------------- | ------------------ | -------------------------------------- |
| A,C  | 1               | 1                  | 1                                      |
| A,D  | 1               | 1                  | 1                                      |
| A,E  | 1               | 1                  | 1                                      |
| A,F  | 1               | 1                  | 1                                      |
| A,G  | 1               | 1                  | 1                                      |
| C,D  | 1               | 1                  | 1                                      |
| C,E  | 1               | 1                  | 1                                      |
| C,F  | 1               | 1                  | 1                                      |
| C,G  | 1               | 1                  | 1                                      |
| D,E  | 1               | 0                  | 0                                      |
| D,F  | 1               | 1                  | 1                                      |
| D,G  | 1               | 0                  | 0                                      |
| E,F  | 1               | 0                  | 0                                      |
| E,G  | 1               | 0                  | 0                                      |
| F,G  | 1               | 0                  | 0                                      |

Jawab:
Cc(B) = 1 + 1 + 1 + 1 + 1 + 1 + 1 + 1 + 1 + 1 = 10