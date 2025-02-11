# 仓库说明

[江协科技](https://space.bilibili.com/383400717) 讲解的 [STM32入门教程-2023版 细致讲解 中文字幕](https://www.bilibili.com/video/BV1th411z7sn) 工程模板

`.vscode`目录包含了vscode的配置，只能用于vscode查找源文件，辅助代码编写

> vscode使用了CL开发的Keil Assistant插件，需要配置 `Keil Assistant.MDK: Uv4 Path`

`DebugConfig`目录定义了调试方式

`library`目录定义了库文件

`start`目录包含启动的汇编程序、外设和内核寄存器定义、系统初始化功能定义

`user`目录是用户编写代码存储位置

`project.uvprojx`文件定义了keil软件需要的设置，包括：

- 使用库文件所需的`USE_STDPERIPH_DRIVER`预处理标志
- 所需的寄存器文件、库文件、中断文件、配置文件

注：
- debug使用STLink作为调试器
- 添加文件时，需要在keil软件中向某一个组添加，以修改`.uvprojx`文件
