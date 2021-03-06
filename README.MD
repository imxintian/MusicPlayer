﻿ XintianMusicPlayer V1.0
========
 ﻿XintianMusicPlayer V1.0是一款开源的基于网易云音乐api的在线音乐播放器。具有音乐搜索、播放、下载、歌词同步显示、个人音乐播放列表同步等功能。

前端界面参照 QQ 音乐网页版进行布局，同时采用了流行的响应式设计，无论是在PC端还是在手机端，均能给您带来原生 app 般的使用体验。

### 相关链接
-----


### 注意事项
-----
#### 关于API文件
由于网易云音乐官方封锁了国外的访问，因此本播放器的 api.php 在海外的空间上可能无法运行(其实有个“你懂的”的功能，请自行挖掘)，建议在国内空间使用。

#### 关于兼容性
本播放器设计支持 IE9及以上的现代浏览器。并且已在 Chrome、firefox、IE11 等浏览器测试使用正常。



#### 关于歌曲
播放器中采用了 [网易云音乐(http://music.163.com/)](http://music.163.com/) 的 api，因此相对应的歌曲版权归网易云音乐所有。支持正版音乐，请使用官方版网易云。


### 更新日志
-----
#### v1.0 Beta `2017/8/28`

- 完善对手机端的适配，新支持 IE9~IE11 浏览器
- 修复 IE11 下点击下载歌曲名字乱码的BUG
- 新增“正在播放”、“播放历史”列表功能
- 新增后台自定义播放列表功能，支持多种列表定义模式
- 新增本地记录用户设置及播放列表功能
- 进度条支持响应点击事件



### 开发文档[待完善]
-----
#### 播放列表DIY教程
本播放器支持后台自定义播放列表。打开 `js/musicList.js`，按照里面的说明对应修改即可。

#### 播放器DIY教程
除了自定义播放列表，本播放器还支持一些 DIY 设定，比如修改 api.php 文件的默认路径、修改搜索框的默认搜索内容等。具体请打开 `js/player.js` 查看

#### rem 变量表
程序中的rem数组用于存储全局变量，具体的成员(部分)及作用见下表：

| 变量名           | 用途                |
| ------------- | ----------------- |
| rem.playlist  | 当前正在播放的播放列表编号     |
| rem.playid    | 正在播放的这首歌在播放列表中的编号 |
| rem.dislist   | 当前显示的列表的列表编号      |
| rem.loadPage  | 搜索功能已加载的页码        |
| rem.wd        | 当前的搜索词            |
| rem.uid       | 当前已同步的用户的网易云 ID   |
| rem.uname     | 已登录用户的用户名         |
| rem.sheetList | 歌单容器操作对象          |
| rem.mainList  | 歌曲列表容器操作对象        |

### 致谢
-----
#### 特别感谢 `网易云音乐`

#### 采用的开源模块
- **Jquery**：js主流开发框架 [http://jquery.com/](http://jquery.com/)
- **layer**：一款强大的web弹层组件 [http://layer.layui.com/](http://layer.layui.com/)
- **mCustomScrollbar**：jQuery自定义滚动条样式插件 [http://manos.malihu.gr/jquery-custom-content-scroller/](http://manos.malihu.gr/jquery-custom-content-scroller/)
- **Let's Kill IE6**：消灭IE [http://overtrue.me](http://overtrue.me)

#### 参考

 [mengkun(http://mkblog.cn)](http://mkblog.cn) 
