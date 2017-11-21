 ###不换行
 ``` bash
 white-space:nowrap; 
 #应用：省略号
 text-overfolw：ellipsis；
 white-space: nowrap;
 overflow: hidden;
 ```

 ###换行，不截断英文，有锯齿
 ``` bash
    word-wrap: break-word;
 ```

### 换行，截断英文，更省空间
``` bash
 word-break:break-all;
```
###另外，只要在CSS中定义了如下句子，可保网页不会再被撑开了。
``` bash
table{table-layout: fixed;}td(word-break: break-all; word-wrap:break-word;)
```