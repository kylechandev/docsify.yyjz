# 定时提醒

从[**Android v4.0**](https://www.coolapk.com/apk/kylec.me.lightbookkeeping)开始，支持设置定时提醒。

?> 从[**Android v6.0**](https://www.coolapk.com/apk/247977)开始，定时提醒功能改为免费功能。

用于设定一个固定的时间，每天在该时间通过系统通知发出记账提醒。帮助避免由于忘记等原因导致的漏记账。 定时提醒功能依赖系统的**通知权限**以及**自启动权限**，请务必确保在系统中打开这两个权限。 这两个权限默认为禁用状态，且必须前往系统设置界面开启。 

- **通知权限**：用于一羽记账通过系统通知发送记账提醒
- **自启动权限**：用于当一羽记账未运行时任然可以发送记账提醒(不能保证100%成功，还需配合省电策略，操作见下)

![定时提醒 - 添加](https://z3.ax1x.com/2021/06/18/R9S6yQ.jpg)

## 收不到提醒？

请在系统设置中查看是否开启了以下权限：

- **发送通知（必须）**
- **自启动（可选）**
- **省电策略-不限制（可选）**

**如何开启？** 以下以小米系统为例**，**在系统设置中**，**找到已安装应用程序**，**找到一羽记账**，**在一羽记账的应用详情界面，开启通知权限以及自启动权限。

!> 开启**自启动**权限也不能100%保证可以在未运行的情况下发出通知提醒，若迫切需要在应用未运行时依然能够发送通知提醒，需要同时设置**省电策略**为不限制（若手机支持设置），否则任然会被系统限制提醒。在未运行应用的情况下，通知提醒的发出时间**有可能**存在2分钟的延迟误差(误差不影响下次的提醒)。<br>![定时提醒 - 后台配置](https://z3.ax1x.com/2021/06/18/R9SHOJ.jpg)

**为了不申请过多的权限(开机自启)，所以当手机重启后，一羽记账可能无法自动重启通知提醒任务。当第一次打开一羽记账后，通知提醒任务将自动重启。**

若仍然无法收到提醒，建议将一羽记账加入系统运行的白名单内，并锁定在后台。 

## 常见问题

> Q: 我可以创建几个定时提醒？ <br>A: 无数个，但不建议创建太多，3个左右即可。

> Q: 如果在提醒时间时，没有运行APP，且没有在后台发出记账提醒通知，此提醒将被如何处理？ <br>A: 若在后台没有成功发出提醒通知，在下次启动APP时，若该提醒设置的时间和当前时间对比误差在10分钟内，将会执行本次提醒通知，反之将自动跳过。

> Q: 小米机型，为什么我的通知被系统折叠了？这导致我无法及时知道系统发送通知。 <br>A: 在系统的通知设置界面，将一羽记账的通知重要性设置为重要。 
>
> ![定时提醒 - 通知](https://z3.ax1x.com/2021/06/18/R9SvY6.jpg)

> Q: 为什么我的手机通知没有显式的提醒，这任然导致我无法即使知道系统发送通知。<br>A: 在系统的通知设置界面中，打开**悬浮通知**开关。同时如果想在锁屏界面可以接收到通知，请打开**锁屏通知**开关。 
>
> ![定时提醒 - 开启通知](https://z3.ax1x.com/2021/06/18/R9SxfK.png)