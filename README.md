# streaming-training
串流計算概念與實作的training

## UI

### 01_BaseUI 建立前端UI與Http後台的雙向訊息傳輸

BaseUI主要想用Socket.io的web-socket的溝通手法來讓後台可以在事件發生的當下，即時以推送(Push)的手法通知前台UI來展現。這個案例想要帶領大家用簡單的手法來體會推(Push)與拉(Pull)兩種手法的融合不僅可以提升使用者的體驗，同時也讓工程師有360度的溝通手法來串連前台與後台。

![01_architecture](https://github.com/erhwenkuo/streaming-training/blob/master/UI/01_BaseUI/architecture.png)


### 02_ScaledUI 建立可Scale-out的後台服務

ScaledUI設計的目的就是展示如何擴展Socket.io的後台服務的專案。為了能夠讓多個Socket.io的nodes可以能夠透明暢通, 我們引進了Redis並透過Redis的PUB/SUB作為所有Socket.io的nodes的訊息管道。

![02_architecture](https://github.com/erhwenkuo/streaming-training/blob/master/UI/02_ScaledUI/architecture.png)

