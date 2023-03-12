# 开放URL Scheme

?> 在[**Android v6.1.2**](https://www.coolapk.com/apk/kylec.me.lightbookkeeping)以上版本支持<br>该功能仅Android版本支持

使用Android系统的URL Scheme，可以通过浏览器或者其他第三方软件跳转到一羽记账App。

部分scheme支持传递参数，参数传递以`?`开始，每个参数以`&`连接，参数形式为`key=value`。

?> 使用`手机浏览器`搜索`yyjz://stat?year=2023&month=2`，体验该功能。

## 启动一羽记账App

> yyjz://home

## 记账页面

> yyjz://newbill

## 记账页面（传递参数）

?> 在[**Android v6.1.3**](https://www.coolapk.com/apk/kylec.me.lightbookkeeping)以上版本支持<br>

> yyjz://addbill

| 参数     | 说明                     | 内容                    | 填写     |
| :------- | :----------------------- | ----------------------- | -------- |
| type     | 账单类型                 | `0支出` `1收入` `2转账` | **必填** |
| book     | 账本名称                 |                         |          |
| category | 分类名称                 |                         |          |
| money    | 账单金额                 |                         |          |
| discount | 优惠金额，仅支出类型可用 |                         |          |
| asset1   | 账户                     |                         |          |
| asset2   | 账户                     |                         |          |
| fee      | 转账手续费               |                         |          |
| remark   | 账单备注                 |                         |          |
| datetime | 日期时间                 |                         |          |
| exbudget | 不计入预算               |                         |          |
| exstat   | 不计入收支               |                         |          |
| tags     | 标签                     |                         |          |

?> 示例：yyjz://addbill?type=0&money=12&category=早餐&remark=豆浆油条

## 统计页面

> yyjz://stat

支持传递参数：

| 参数  | 说明                               |
| :---- | :--------------------------------- |
| year  | 年份（可选，2010 ~ currentYear+1） |
| month | 月份（可选，1 ~ 12）               |

?> 完整示例：yyjz://stat?year=2023&month=2

## 日历页面

> yyjz://calendar