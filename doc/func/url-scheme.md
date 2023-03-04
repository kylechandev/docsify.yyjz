# 开放URL Scheme

?> 在**[Android v6.1.2](https://www.coolapk.com/apk/kylec.me.lightbookkeeping)**以上版本支持。<br>该功能仅Android版本支持

使用Android系统的URL Scheme，可以通过浏览器或者其他第三方软件跳转到一羽记账App。

部分scheme支持传递参数，参数传递以`?`开始，每个参数以`&`连接，参数形式为`key=value`。

?> 使用`手机浏览器`搜索`yyjz://stat?year=2023&month=2`，体验该功能。

## 启动一羽记账App

> yyjz://home

## 记账页面

> yyjz://newbill

## 记账页面（传递参数）

> yyjz://addbill

| 参数     | 说明 |
| -------- | ---- |
| 暂未上线 |      |

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