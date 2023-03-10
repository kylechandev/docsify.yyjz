# 权限申明 (Android)

<font color=gray>使用了哪些权限？为什么需要这些权限？</font>

- **【完全的网络访问权限】**：自动检测版本更新、WebDAV备份 - 自动授权
- **【查看网络连接】**：根据当前网络的状态是否可用来判断是否需要执行自动版本更新检测 - 自动授权
- **【查看WLAN链接】**：应用用户分析统计，用于标识一个设备；
- **【读取共享存储空间中的内容】**：导入账单数据时读取文件的内容 - 需要手动授权
- **【读取共享存储空间中的图片文件】**：同上，适配Android13 - 需要手动授权
- **【使用指纹硬件】** 应用安全-指纹识别(低版本Rom) - 自动授权
- **【运行前台服务】**：桌面小部件(Android8.0及以上) - 自动授权
- **【防止手机休眠】**：桌面小部件(原生需要)、WebDAV备份(后台任务进程，即用即停) - 自动授权
- **【拍摄照片和视频】**：添加图片备注时，直接使用系统相机拍照 - 需要手动授权
- 【**显示通知**】：通知权限，适配Android13，发出记账提醒通知 - 需手动授权

## 隐私问题

在使用过程中，完全无需担心隐私问题。

第一，一羽记账根本没有写文件到非私有目录的权限（除了备份文件的授权目录，如果使用的话）。

第二，一羽记账根本没法读取设备的存储文件（除了导入与导出，主动从文件管理器中选择文件）。

欢迎监督~🤓