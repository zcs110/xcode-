# xcode-
如何找到XCode插件位置
1.打开xcode插件所在的目录：
~/{当前用户名}/library/Application Support/Developer/Shared/Xcode/Plug-ins
2.选择已经安装的插件例如VVDocument，右键点击show package contents，
3.找到info.plist 文件，找到DVTPlugInCompatibilityUUIDs的项目，
4.添加C4A681B0-4A26-480E-93EC-1218098B9AA0（当前xcode的一个号码），这个号码怎么得到？

 在终端执行 defaults read /Applications/Xcode.app/Contents/Info DVTPlugInCompatibilityUUID 即可
5.再右键“打开报内容”双击contents\MacOS目录下的一个黑色图标，会打开终端窗口，最后打印“进程已完成”之类，
重启xcode
 
