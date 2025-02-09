# 我的电视·〇

电视网络视频播放软件，可以自定义视频源

[my-tv-0](https://github.com/lizongying/my-tv-0)

## 使用

* 遥控器左键/触屏单击打开节目列表
* 遥控器右键/触屏双击打开配置
* 遥控器返回键关闭节目列表/配置
* 打开配置页后，配置地址后并确认，更新节目列表

目前支持的配置格式：

* txt
    ```
    组名,#genre#
    标题,视频地址
    ```
* m3u
    ```
    #EXTM3U
    #EXTINF:-1 tvg-name="标准标题" tvg-logo="图标" group-title="组名",标题
    视频地址
    ```
* json
    ```json
    [
      {
        "group": "组名",
        "logo": "图标",
        "name": "标准标题",
        "title": "标题",
        "uris": [
          "视频地址"
        ]
      }
    ]
    ```

推荐配合使用 [my-tv-server](https://github.com/lizongying/my-tv-server)

下载安装 [releases](https://github.com/lizongying/my-tv-0/releases/)

更多地址 [my-tv](https://lyrics.run/my-tv-0.html)

![image](./screenshots/img.png)
![image](./screenshots/img_1.png)

## 更新日志

### v1.0.9

* 减小频道数字文字大小
* 播放时背景颜色为黑色

### v1.0.8

* 点击节目列表/菜单以外区域，自动隐藏节目列表/菜单
* 解决部分情况下崩溃问题

### v1.0.7

* 支持rtsp直播
* 支持循环播放
* 支持txt/m3u视频源

### v1.0.6

* 修复视频可能无声音的问题
* 修复视频可能无法播放的问题

### v1.0.5

* 修复频道配置错误时可能崩溃的问题
* 修复更新频道配置时可能不生效的问题
* 修复图标为空时可能崩溃的问题

### v1.0.4

* 在触屏设备上双击打开节目列表
* 支持自动更新

### v1.0.3

* 保存上次频道

### v1.0.2

* 改变部分样式

### v1.0.1

* 支持返回键退出
* 支持基本的视频源配置

### v1.0.0

* 基本视频播放

## 其他

小米电视可以使用小米电视助手进行安装

如电视可以启用ADB，也可以通过ADB进行安装：

```shell
adb install my-tv-0.apk
```

## TODO

* 音量不同
* 收藏夹
* 节目增加预告
* 频道列表优化
* 节目列表焦点消失的问题

## 赞赏

![image](./screenshots/appreciate.jpeg)