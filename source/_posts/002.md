---
title: 解决EXE应用程序图标丢失
date: 2023-03-14 09:51:43
tags: 电脑相关
---

1.使用快捷键键 "Win+R" 打开运行窗口，输入 "cmd" 确定打开命令提示符

2.分别输入以下代码

```
taskkill /im explorer.exe /f
cd /d %userprofile%\appdata\local
del iconcache.db /a
start explorer.exe
exit
```
