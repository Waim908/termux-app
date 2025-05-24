# 最新版

## 1.5.0.1 稳定版

做出如下修改：

1.彻底修复深色模式下字体无法显示问题，深色主题修复（除了部分背景问题，字体基本全部正常显示）

2.在主界面添加了`操作提示`按钮

3.修复x11依赖安装脚本`install`

4.修复进程脚本`collect_process_info`只显示前十个的问题

5.部分x11首选项默认设置的更改

6.修改app名称为`终端与termux-x11`

7.悬浮球点击关闭x11按钮后弹出提升是否确认关闭，防止x11进程被误触停止

### 此稳定版在jiaxinchen更新app版本号之前不再进行更新


# 如何构建

`git clone -b master-x11-submodule https://github.com/Waim908/termux-app &&
cd termux-app &&
git submodule update --init --recursive &&
./gradlew syncDebugLIbJars &&
./gradlew assembleDebug`

如果构建失败考虑fork此仓库使用github action