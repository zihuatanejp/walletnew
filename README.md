# walletnew
true chain light wallet: it is a react-native project

## 初始化方式（安装运行）
----
### 面向普通用户
### 面向开发者
----
先配置好环境（已有环境可跳过），  
参考这里: [搭建rn开发环境](https://reactnative.cn/docs/getting-started.html)

```
下载安装项目:
> git clone https://github.com/zihuatanejp/walletnew.git

> cd walletnew //进入项目测试

> npm install //安装项目依赖包

//需要对react-native-crypto包特别对待：
//先卸载
> npm uninstall --save-dev tradle/rn-nodeify
> npm uninstall --save tradle/rn-nodeify
> react-native unlink react-native-randombytes
> npm uninstall react-native-randombytes
> npm uninstall react-native-crypto

//重装:
> npm install --save react-native-crypto
> npm install --save react-native-randombytes
> react-native link react-native-randombytes
> npm install --save-dev tradle/rn-nodeify
> npm install --save tradle/rn-nodeify
//打开powershell(如果是windows用户，然后进入项目目录)
> ./node_modules/.bin/rn-nodeify --hack --install //重写覆盖已有的包内容

运行起来：
	在ios上运行app:
		1.
		> cd truewallet
		> react-native run-ios
		或者在xcode里 打开 ios/truewallet.xcodeproj
	在安卓上运行app:
		> react-native run-android


调试项目：
模拟器：
	ios上 Cmd+R：刷新重载 Cmd+D:调出开发者菜单
	安卓上 双击R：刷新重载 
  > adb shell input keyevent 82 //调出开发者菜单
  

真机： 摇晃手机调出开发者菜单 -> reload

```
