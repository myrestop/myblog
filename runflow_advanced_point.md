# The fully advanced manual of the productivity application RunFlow

Welcome to our advanced manual of the RunFlow, if you don't know RunFlow yet, we recommend you read our [fundamental manual](runflow_basic_point.md) first.

### Searching Files

Appending `len` parameter to filter files by size, such as: `len:1kb-2kb`, `len:3mb-5mb` etc.

![find_file](images/find_file_with_size_filter_enus.gif)

> `**` can match multi-level directories. For an instance, finding files which start with `test` in the folder `folder_a`, we can input like this: `folder_a/**/test`.

### Calculator

We have two preset irrational numbers `e` and `pi`.

![pi_and_e](images/pi_and_e_enus.gif)

Calculating big numbers, if you want to calculate `9999999999999999999*9999999999999999999`, there is no result if you input it directly like this. We should append a `d` parameter after the number, like this: `9999999999999999999d*9999999999999999999d`.

![calc_big_number](images/calc_big_number_enus.gif)

### 解散文件夹

假设我们有下方示例的一个文件夹，现在我们需要删除文件夹，把所有文件提到同一级，我们就可以使用 `folderunwrap`。

```text
文件夹
├─文本文件_01.txt
├─文本文件_02.txt     
├─文件夹01
│ ├─文本文件_03.txt
│ └─文本文件_04.txt
└─文件夹02
  └─文件夹03
    ├─文本文件_05.txt
    └─文本文件_06.txt
```

解散文件夹后都在同一个目录级别：

```text
文本文件_01.txt
文本文件_02.txt
文本文件_03.txt
文本文件_04.txt
文本文件_05.txt
文本文件_06.txt
```

![unwrap_folder](../images/unwrap_folder_zhcn.gif)

### 独立窗口运行

![separate_window](../images/separate_window_zhcn.gif)

### 导入导出数据

我们支持导出JSON格式的数据，同样导入数据也需要是JSON格式的。

### 数据同步

##### 本地同步服务

基于本地的同步服务是我们内置的功能，它依赖于第三方的云盘服务，比如OneDrive、iCloud、Google Drive、小米云盘、百度云盘、阿里云盘等等。

这里我以我常用的OneDrive作为示例，其他云盘的同步方法也都一样，我们可以先在OneDrive中新建一个 `MyFlow` 的文件夹用来存储需要同步的数据，然后打开RunFlow数据同步的设置页面，开启基于本地的数据同步服务，并设置数据所在文件夹即可。

![data_sync](../images/data_sync_zhcn.gif)

> 偷偷告诉你，开启数据同步服务可以同步剪贴板。

### 定时任务

在热点事件的设置页面中，我们可以通过Cron表达式来设置定时任务，比如定时清理电脑垃圾回收站、定期重建文件索引等等。

![cron](../images/cron_zhcn.gif)

这里简单解释一下上面的Cron表达式：

| 秒 | 分 | 时  | 天 | 月份 | 星期 | 解析          |
|---|---|----|---|----|----|-------------|
| 0 | 0 | 12 | * | *  | *  | 每天中午的12点执行  |
| 0 | 0 | 12 | * | *  | 1  | 每周一的中午12点执行 |

<br/>

> 了解等多Cron表达式，可以[点击这里](https://baike.baidu.com/item/cron)。

### 结语

本工具内置常见的进阶功能就介绍到这里了，如果您还想了解更多功能，可以到我们的[插件商店](https://myrest.top/store/plugin)看看，如果您是一名开发者，欢迎阅读我们的开发者篇手册，也欢迎您来提交插件。
