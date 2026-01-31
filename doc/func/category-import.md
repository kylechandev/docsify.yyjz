# 导入分类 (Android)

?> iOS/HarmonyOS NEXT 端暂不支持此功能

通过系统文件管理器、微信、QQ等方式选择`分类导出文件`，并选择文件打开方式为`一羽记账的导入分类`。具体方式同[导入账单数据](doc/data-manage/import-data.md#import-way)完全一致。

文件打开后会自动进入一羽记账的分类管理界面，并执行导入。

## 注意事项

导入数据中，分类数据必须满足以下条件才会被导入：

- 分类名称不为空
- 图标必须合法（一羽记账内置图标，Androidv5.5.0后支持自定义的图标Url链接）
- 已有分类数据中不存在（自动过滤）

不支持导入分类颜色。

## 导出文件位置

```
Android/data/data/kylec.me.lightbookkeeping/YiYuJiZhang/Export/Category
```