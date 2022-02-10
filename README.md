# UnityDirtyCompiler 脏脚本编译工具
### >> 该工具解决了什么问题
对客户端程序员而言，有时只在脚本里加入一句Log，但是刷新编辑器却要耗时15秒以上（大工程就需要更久）。
使用此工具进行编译，Unity只会编译脚本所在的程序集。

（以我个人工程举例：刷新耗时可从15s降至1s）

### >> 环境
支持Unity2019.4 / 2021.2

### >> 使用说明
1. 下载zip源码
2. 将源码解压到工程的Assets目录里的任意位置
3. 编译脚本时，使用CTRL+T进行刷新即可

### >> 注意事项
1. 如有新增/移除文件，请使用CTRL+R刷新
2. 只支持Runtime代码

### >> 原理
1. 监控脏脚本（修改后的脚本）
2. 调用官方编译接口
3. 编译完成后触发编译完成事件
