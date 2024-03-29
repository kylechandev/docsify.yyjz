# 存钱计划

从[**Androidv5.3.0**]版本开始，提供存钱计划功能。

支持三种存钱模式：

> * 递增存钱
> * 定额存钱
> * 自由存钱

![存钱计划](https://s1.ax1x.com/2023/01/10/pSejckV.jpg)

### 存钱模式

### 递增存钱

> 设定`存钱周期`，`初始存钱金额`，每次`递增存钱金额`，`每/周/月`存一次钱

比较常见的递增存钱方式有：

1. 365天存钱
   
   > 一年365天，每天按天数存钱。<br>例如第一天存1元，第二天存2元，第365天存365元。<br>一年累计可存下66795元。

2. 52周存钱
   
   > 将一年分成52周，起始周存10元，往后每周在上周的基础上多存10元。<br>例如第一周存10元，第二周存20元，第52周存520元。<br>一年累计可存下13780元。

?> 一羽记账已内置以上两种递增存钱模式

### 定额存钱

同`递增存钱模式`大致相同，但每次存钱金额都固定不变。

### 自由存钱

不设时间周期限制，不限制存钱金额，存钱时机由自己决定。

## 自动记录

> 非自由存钱模式下可用<font color=orange>（此功能为Pro功能）</font>

到达存钱日期时，App会自动进行存钱操作，无需再次手动操作存钱。

## 存钱关联账户

添加存钱计划时，可设置存钱的转出转入账户，这样在每次存钱后都会自动额外生成一笔存钱账户间的转账账单。（需要开启资产账户功能`记账设置->记账界面功能自定义`）

> 因为存钱本质上就是将自己的钱从一个账户，转移到一个固定的存钱账户，所以可以将存钱定义为一个转账逻辑。