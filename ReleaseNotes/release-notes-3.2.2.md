# PLDroidShortVideo Release Notes for 3.2.2

### 简介

PLDroidShortVideo 是七牛推出的一款适用于 Android 平台的短视频 SDK，提供了包括美颜、滤镜、水印、断点录制、分段回删、视频编辑、混音特效、本地/云端存储在内的多种功能，支持高度定制以及二次开发。

### 版本

* 发布 pldroid-shortvideo-3.2.2.jar
* 新增 libQMedia.so
* 移除 armeabi 支持

### 功能

* 视频录制支持白平衡手动设置
* 视频录制支持背景音乐选择是否循环

### 缺陷

* 修复 Android10 及以上版本无法进行屏幕录制的问题
* 修复视频拼图以及区域剪裁失效的问题
* 修复个别机型转码崩溃问题
* 修复某些机型上软编出现的崩溃问题

### 注意事项

* 从 v3.1.0 版本开始，需要在 Application 中初始化 sdk：

```java
PLShortVideoEnv.init(getApplicationContext());
```

* 七牛短视频 SDK 自 v3.0.0 版本起, 划分为精简版、基础版、进阶版、专业版。不同版本 SDK 可以使用的功能点数量有差别，请按照购买的 License 版本使用对应的短视频 SDK 版本。
* 上传 SDK 的依赖需要更新到如下版本：

```java
compile 'com.qiniu:qiniu-android-sdk:7.6.4'
```


