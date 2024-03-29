# 数据云同步

## 介绍

从[**Android v5.0**]开始，支持数据云同步功能。仅<font color=orange>永久会员(云同步)</font>可用。

支持自动同步数据到一羽记账的云服务器中。

**有无网络时都能够记录任何数据，无网络不影响**，等网络恢复后，通过在首页下拉刷新即可完成数据云同步。

云同步在多设备使用时非常方便，在一台设备上的任何修改/添加/删除操作，只需要在另一台设备上`下拉刷新`一次，即可完成多设备数据同步。

## 数据同步状态

在首页的「我的」页面，如果页面右上角出现了「☁️」图标，并且有现`小红点`以及`数字`时，表示当前存在`未同步完成`的账单<font color=gray size=1>（数字代表未同步的账单数量）</font>。点击「☁️」图标后，可以手动执行一次数据云同步。

如果右上角没有显示任何内容，则说明当前`数据云同步`状态一切正常~

![示例 - 存在未同步数据](https://z3.ax1x.com/2021/09/29/45azuV.jpg)

服务器中的数据永久保存，且拥有自动备份策略，无需担心数据丢失问题。

同时`在一羽记账中删除的数据`在云服务器中有一定的缓存期，等待缓存期结束后才会真正的从服务器彻底抹除掉数据。

所以如果有误操作删除数据，可以[联系我](doc/other/contact.md)，如果还在缓存期内，是可以帮助恢复误删除数据的。

## 启用「数据云同步」后

> 数据将始终自动与云端保持同步，以防冲突，本地备份或WebDAV云备份的恢复备份将被自动忽略<br><br>使用云同步后，也无需再关心备份，数据将实时自动与云端同步保存<br><br>但仍可以继续备份，以保留备份文件在身边作为保险