# YzyFFmpegPlayer
利用ffmpeg打造万能播放器  
- 如果觉得有用，不吝啬在右上角给我一个Star。谢谢！！  
![](https://raw.githubusercontent.com/yzytmac/yzytmac.github.io/master/images/star.png)  
遇到的问题：  
1、生成头文件时无法确定Surface的签名，将SDK/platforms/android-22/android.jar配置到classpath中即可，因为Surface是Android中的不是java中的，所以不配置的话识别不了，做NDK开发时还会遇到Bitmap无法确定签名也是这个原因  
2、编译的时候c代码中总会有一些变量无法解析，可以检查symbol and path有没有正确引入相应的头文件，如果都正确引用了还报红那么就project->clean一下就好了，一般都能解决  
3、现在编译好的库只支持armeabi的cpu，也就是几年前的cpu，还没编译出armeabi_v7a及以上的库，所以现在的旗舰手机一般用不了，后面会继续编译  
4、播放过程中会出现闪退现象，log也看不懂，这个bug后续将解决，如果有大神知道问题所在欢迎指教  
5、目前只实现的视频的播放，还没有声音，因为声音解码这一块还没来得及做，最近较忙，等闲了再说。  
邮箱：yzytmac@163.com
