### React Native 练习(ios版本领先)


使用到的组件

[底部导航菜单](https://github.com/happypancake/react-native-tab-navigator): react-native-tab-navigator

[滑动tab](https://github.com/skv-headless/react-native-scrollable-tab-view): react-native-scrollable-tab-view


### 问题汇总

1、执行 react-native run-android 时下载 gradle-2.14.1-all.zip 很慢

错误示范：本来是 gradle-3.3 版本，在命令行 执行 react-native run-android 后发现速度太慢，强制结束下载，报错如下：

![Alt 错误](./logs/01.png)

非正常方法：直接把 ~/.gradle 文件删除了(记得删缓存)  
其实只要修改 build.gradle 文件就可以了

初次下载的话，可以参考下面的方法

[参考](http://www.cnblogs.com/Ave-Maria/p/6274563.html)  
gradle zip 包 都比较大, 可以将它下载到本地，修改 gradle-wrapper.properties 中的地址  
无语的是用浏览器下载也是龟速，只有去网上找国内的镜像文件了...

2、