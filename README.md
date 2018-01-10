# YzyFFmpegPlayer
利用ffmpeg打造万能播放器  
遇到的问题：  
1、生成头文件时无法确定Surface的签名，将SDK/platforms/android-22/android.jar配置到classpath中即可  
2、编译的时候c代码中总会有一些变量无法解析，可以检查symbol and path有没有正确引入相应的头文件，如果都正确引用了还报红那么就project->clean一下就好了  
