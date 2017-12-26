---
layout: default
title:  "欲練Jekyll神功，必先自裝Ruby"
---

---
+# mermaid绘图
 +****
 +第一种方法：无需插件在jekyll嵌入图表，只需在网页上引用mermaid
 +
 +```html
 +<script src="https://cdn.bootcss.com/mermaid/7.1.0/mermaid.min.js"></script>
 +```
 +```html
 +<div class="mermaid">
 +graph TD;
 +    早餐-->苹果;
 +    早餐-->牛奶;
 +    苹果-->一个就好;
 +    牛奶-->最好不要空腹饮用;
 +</div>
 +```
 +<div class="mermaid">
 +graph TD;
 +    早餐-->苹果;
 +    早餐-->牛奶;
 +    苹果-->一个就好;
 +    牛奶-->最好不要空腹饮用;
 +</div>
 +
 +第二种方法：jekyll-mermaid Plugin
 +
 +```html
 +{% raw %}
 +{% mermaid %}
 +　　　dateFormat　YYYY-MM-DD
 +　　　title Adding GANTT diagram functionality to mermaid
 +　　　section A section
 +　　　Completed task　　:done, des1, 2014-01-06,2014-01-08
 +　　　Active task 　　　　:active, des2, 2014-01-09, 3d
 +　　　future task 　　　　:　　　  des3, after des2, 5d
 +　　　future task2　　　　:　　　  des4, after des3, 5d
 +　　　section Critical tasks
 +　　　Completed task in the critical line　:crit, done, 2014-01-06,24h
 +　　　Implement parser and json　　　　　　:crit, done, after des1, 2d
 +　　　Create tests for parser　　　　　　　:crit, active, 3d
 +　　　Future task in critical line　　　　　:crit, 5d
 +　　　Create tests for renderer　　　　　　:2d
 +　　　Add to ,mermaid　　　　　　　　　　　:1d
 +{% endmermaid %}
 +{% endraw %}
 +```
 +{% mermaid %}
 +gantt
 +　　　dateFormat　YYYY-MM-DD
 +　　　title Adding GANTT diagram functionality to mermaid
 +　　　section A section
 +　　　Completed task　　:done, des1, 2014-01-06,2014-01-08
 +　　　Active task 　　　　:active, des2, 2014-01-09, 3d
 +　　　future task 　　　　:　　　  des3, after des2, 5d
 +　　　future task2　　　　:　　　  des4, after des3, 5d
 +　　　section Critical tasks
 +　　　Completed task in the critical line　:crit, done, 2014-01-06,24h
 +　　　Implement parser and json　　　　　　:crit, done, after des1, 2d
 +　　　Create tests for parser　　　　　　　:crit, active, 3d
 +　　　Future task in critical line　　　　　:crit, 5d
 +　　　Create tests for renderer　　　　　　:2d
 +　　　Add to ,mermaid　　　　　　　　　　　:1d
 +{% endmermaid %}
 +
 +
 +mermaid参考手册：<https://github.com/knsv/mermaid>
 +
 ---