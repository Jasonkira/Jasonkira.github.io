---
layout: default
title:  "李杨成的第一篇博客"
---
- [x] 早餐爱好
  - [x] 1.牛奶和面包
  - [ ] 2.泡面加火腿肠
  - [x] 3.白粥
  - [x] 4.不吃


```
graph TD
    A[Christimas] -->B(Go shopping)
    B -->C[let me think]
    C -->|One| D[ipad]
    C -->|two| E[iphone]
    C -->|Three| F[camera]
    C -->|Four| G[flower]
```
```

graph LR
A-->B
```

```
sequenceDiagram
Jason->>Jackson: How are you?
Jackson->>Jason: Great!
```

```
gantt
dateFormat YYYY-MM-DD
title 产品计划表
section 初期阶段
明确需求:2016-03-01, 10d
section 中期阶段
跟进开发:2016-03-11, 15d
section 后期阶段
走查调查:2016-03-20, 9d
section 收尾阶段
撰写论文:2016-03-29, 8d
```
```
gantt
        dateFormat  YYYY-MM-DD
        title Adding GANTT diagram functionality to mermaid
        section A section
        Completed task            :done,    des1, 2014-01-06,2014-01-08
        Active task               :active,  des2, 2014-01-09, 3d
        Future task               :         des3, after des2, 5d
        Future task2               :         des4, after des3, 5d
        section Critical tasks
        Completed task in the critical line :crit, done, 2014-01-06,24h
        Implement parser and jison          :crit, done, after des1, 2d
        Create tests for parser             :crit, active, 3d
        Future task in critical line        :crit, 5d
        Create tests for renderer           :2d
        Add to mermaid                      :1d
```