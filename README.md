# LoggerView
# 可以在APP上查看log日志的工具类
### 使用方法，把Logger.java文件拷贝到你项目的工具包下面即可
初始化方法：
在application 的 onCreate() 方法初始化
```
Logger.init(this);
```
## 在APP上唤起log日志悬浮窗界面方法，点击事件，屏幕任意位置快速点击3下，然后慢速点击3下，再快速点击3下（SOS的摩斯电码）
## 以上操作是为了增加误触难度，（再次按上面方法可以关闭）新增长按悬浮窗标题栏关闭悬浮窗
## 在log界面显示的时候，若要唤起log筛选器，在屏幕顶部200像素内，快速单击5下（新增点击悬浮窗标题栏也可唤起）；

## 本工具类具有功能：
  ### 1.任意界面可唤起日志悬浮窗，显示app即时日志，可过滤筛选日志，可单击日志放大，清空；
  ### 2.捕捉app崩溃日志。即时弹窗显示崩溃信息，分2种情况，activity启动时崩溃会打开浏览器展示崩溃日志，其它崩溃直接弹窗；
  ### 3.兼容其它异常捕捉框架（测试中。。。）
  ### 4.若遇到view在切后台时空白等跟本工具类冲突的情况，请在activity上注解@Logger.IgnoreLoggerView不展示悬浮窗

