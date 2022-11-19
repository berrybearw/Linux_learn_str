# Linux_learn_str
字串處理簡介

cut 取出部分字串
---

從一列取出一部分

cut -c2 dataf1

抽出 dataf1 每一列出現的 第 2 個字元

cut -c3-10 data1

抽出 data1 每一列 3 到 10 字元

cut -c9- data1

每一列 從 9 之後全部字元

cut -1-3,22 data1

每一列 1 到 3 字元 , 與 22 以後全部字元 

cut -d: -f1 /etc/data1

找出 data1 第一欄位 , -d: 用 : 分隔符 , -f1 第一欄

cut -d: -f3,4 /etc/data1

找出 data1 第 3 和 4 欄位

sort 排序
---

sort data1

升冪 ( 由大到小 )

sort -r data1 

降冪 ( 由小到大 )

sort -n data1

用數值比較

sort -n +2 data1

跳過前兩欄 用數值比較

sort -nr +2 -t: data1

-t: 用 : 分隔符號區分

wc 計算字串長度
---

wc

wc -l dataf1

顯示檔案內共有幾列

wc -c file

顯示共有多少字元

wc -w file

顯示共有多少單字

