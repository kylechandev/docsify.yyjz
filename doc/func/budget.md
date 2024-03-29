# 预算管理

## 概况

预算管理管理共分为三类：

1. 月总预算
2. 日均预算（根据月总预算自动设置，不支持手动设置）
3. 分类预算

?> 从[**Android v4.1.5**]版本开始，支持每月的预算相互独立，可单独设置每个月的预算。<br>新的月份到来时，会自动沿用上个月的预算（如果上个月有设置预算），*需要在新的月份里启动一次一羽记账*。

### 修改预算额度

- 月总预算：**点击**预算管理界面顶部的月预算卡片
- 分类预算：点击分类预算的`剩余额度`区域，即可修改预算额度

### 删除预算

- 月总预算：**长按**预算管理界面顶部的月预算卡片
- 分类预算：分类预算详情界面右上角的删除按钮

## 剩余日均  :id=remain-daily-average

计算方法是：剩余预算（**排除今日支出**）/ 月剩余天数。

!> 注意！是排除今日支出后的剩余预算！<br>若剩余预算降为0，则剩余日均始终为0<br>当今日支出超出上述计算的剩余日均时，代表今日超支，剩余日均的计算将转为实时更新。

为什么要排除今日支出？ <br>因为如果不排除掉今日支出，每次进行记账后，剩余日均都将发生变化，这就导致剩余日均没有任何的参考价值，到底今天还剩下多少预算可用？

这样，我们就可以真正通过将`今日支出`和`剩余日均`做对比，看看今天的支出有没有超日预算了。