# Hide My Applist
## About this module  
Although "It is incorrect to detect specific app's installation", yet not every app using root provides random packagename support.
In this case, detected apps that use root (such as Fake Location and Storage Isolation) is equal to detected root itself.  
At the same time, some "smart" apps use various loopholes to acquire your applist, so that it can draw a persona for you.  
This module provides some methods to test whether you have already hidden your applist nicely.  
Also, it can work as an Xposed module to hide some apps or reject applist requests to protect your privacy.   
Attension: Xposed API version lower than 93 is NOT supported due to a permission problem  
## Compilation
This project uses Hidden API, so you should replace android.jar in Android Studio. [Reference](https://github.com/anggrayudi/android-hidden-api)  
## Update Log
V1.3.1  
+ Performance optimization  

V1.3  
+ Downgrade minSdkVersion  
+ Add new detection methods and interception methods  
+ Modifying templates takes effect in real time without restarting target apps (except for file detections)  
+ UI redesign with more help information in about page  
+ Due to the big changes to V1.1, if there are problems please uninstall and reinstall the module  

V1.1  
+ Add exclude self support  

## 关于该模块  
虽然“检测安装的应用是不正确的做法”，而且很蠢，但是并不是所有的插件类应用都提供了随机包名支持。在这种情况下，检测到安装了root类应用（如Fake Location、存储重定向）与检测到了root本身区别不大。（会使用检测手段的app可不会认为你是在“我就蹭蹭不进去”）  
与此同时，部分“不安分”的app会使用各种漏洞绕过系统权限来获取你的应用列表，从而对你建立用户画像。（如陈叔叔将安装了V2Ray的用户分为一类）  
该模块提供了一些检测方式用于测试您是否成功的隐藏了带有root印记的包名，如Magisk/Edxposed Manager。  
同时可作为Xposed模块用于隐藏应用列表或特定应用，保护你的隐私。  
注意：由于一个权限问题，Xposed API至少为93才能正常使用该模块  
## 更新日志
V1.3.1  
+ 性能优化  

V1.3  
+ 支持更低Android版本  
+ 增加新的检测方式和拦截方式  
+ 修改模板实时生效，无需重启目标应用（除File detections）  
+ UI重修，关于页面添加更多使用帮助  
+ 由于较V1.1改动大，遇到问题请卸载重装模块  

V1.1  
+ 增加了排除自身功能  

## TODO
+ Solve MODE_WORLDREADABLE problem
+ Downgrade Xposed API version
+ Fix webview problems