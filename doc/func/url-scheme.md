# 开放URL Scheme

?> 在[**Android v6.1.2**]以上版本支持<br>该功能仅Android版本支持

使用Android系统的URL Scheme，可以通过浏览器或者其他第三方软件跳转到一羽记账App。

部分scheme支持传递参数，参数传递以`?`开始，每个参数以`&`连接，参数形式为`key=value`。

?> 使用`手机浏览器`搜索`yyjz://stat?year=2023&month=2`，体验该功能。

## 启动一羽记账App

> yyjz://home

## 记账页面

> yyjz://newbill

## 记账页面（传递参数） :id=addbill

?> 在[**Android v6.1.3**]以上版本支持<br>

<font color=gray size=2>* 手机端建议横屏查看</font>

> yyjz://addbill

| 参数        | 说明                | 必须为                                                                                                                    | 填写       |
|:--------- |:----------------- | ---------------------------------------------------------------------------------------------------------------------- | -------- |
| type      | 账单类型              | `0 - 支出`<br>`1 - 收入`<br>`2 - 转账`<br>v6.3.2新增类型：<br>`3 - 报销`<br>`9 - 应收账款`                                              | **必填**   |
| book      | 账本名               | <font color=gray size=2>不填则为默认账本</font>                                                                                | 可选       |
| category  | 分类名               | <font color=gray size=2>收支必填，转账不填</font>                                                                               | *根据账单类型* |
| money     | 账单金额              | <font color=gray size=2>不超过App内金额限制（88888888）</font>                                                                   | **必填**   |
| discount  | 优惠金额              | <font color=gray size=2>仅支出类型，不能超过账单金额</font>                                                                          | 可选       |
| asset1    | 账户                | <font color=gray size=2>收支可选填，转账必填</font>                                                                              | *根据账单类型* |
| asset2    | 账户                | <font color=gray size=2>收支不填，转账必填</font>                                                                               | *根据账单类型* |
| fee       | 转账手续费             | <font color=gray size=2>收支不填，转账可选填</font>                                                                              | 可选       |
| remark    | 账单备注              | <font color=gray size=2>任意文本，不超过App内长度限制（80）</font>                                                                    | 可选       |
| datetime  | 日期时间              | ex: `2023-03-12`<br><br> `2023-03-12 22:01:51`<br><br> `2023-03-12 22:02`<br><font color=gray size=2>不填则默认为当前时间</font> | 可选       |
| exbudget  | 不计入预算             | <font color=gray size=2>仅支出类型可用，1表示不计入预算，非1表示计入，默认计入</font>                                                            | 可选       |
| exstat    | 不计入收支             | <font color=gray size=2>仅收支类型可用，1表示不计入收支，非1表示计入，默认计入</font>                                                            | 可选       |
| tags      | 标签名               | <font color=gray size=2>多个标签用`英文逗号,`分隔，总个数不超过App内限制（4）</font>                                                          | 可选       |
| showsheet | 打开确认记账弹框（可继续编辑记账） | v6.3.2新增：<br><font color=gray size=2>1表示弹窗确认记账，非1表示不弹窗直接完成记账，默认不弹窗<br>如果此值传1，部分参数例如分类账户可以不传递，在弹出的窗口在再进行手动设置</font>     | 可选       |

?> 示例：yyjz://addbill?type=0&money=12&category=早餐&remark=豆浆油条

showsheet参数效果图：

![showsheet参数效果图](https://z1.ax1x.com/2023/11/13/piJlIkn.jpg)

账户参数支持自动保存映射，后续传参相同账户名可以自动映射到App内真实账户。

点击右上角`开发者`按钮可以自定义设置。

## 统计页面

> yyjz://stat

支持传递参数：

| 参数    | 说明                          |
|:----- |:--------------------------- |
| year  | 年份（可选，2010 ~ currentYear+1） |
| month | 月份（可选，1 ~ 12）               |

?> 完整示例：yyjz://stat?year=2023&month=2

## 日历页面

> yyjz://calendar