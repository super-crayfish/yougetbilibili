you-get批量下载bilibili视频
本人cmd >you-get -V
you-get: version 0.4.1432, a tiny downloader that scrapes the web.
python安装 you-get 库和使用方法
https://www.cnblogs.com/bigpig369/articles/8785761.html
xpath安装教程
https://www.cnblogs.com/duanlinxiao/p/11624431.html
安装完成以后
https://space.bilibili.com/472422994/video
测试xpath  开发模式打开，ctrl+shift+alt+x 
黑色窗口输入
//*[@id="submit-video-list"]/ul/li/a/@href
或者
//*[@id="multi_page"]/div/ul/li/a/@href

取得结果
//www.bilibili.com/video/BV1tV411v7KE
//www.bilibili.com/video/BV12h411r7n5
//www.bilibili.com/video/BV1UX4y1P76Y
//www.bilibili.com/video/BV1S5411E7xi
//www.bilibili.com/video/BV1eV411t7yR
//www.bilibili.com/video/BV1hK411u7m5
//www.bilibili.com/video/BV1DK411M723
//www.bilibili.com/video/BV1Jo4y1Z7bo
//www.bilibili.com/video/BV1of4y1e7TK
//www.bilibili.com/video/BV1cp4y167MF

在桌面新建  you-get.bat文件 F:/Download 是我的下载路径，分隔符上面是bat文件内容

@echo off
cd /d F:/Download
echo 当前路径是 %cd%
you-get -o F:/Download https://www.bilibili.com/video/BV1tV411v7KE https://www.bilibili.com/video/BV12h411r7n5        




升级版本
  升级批量下载 ?p=页码数视频   
  提交 you-get.bat  文件，需要根据自己需求填写下载视频号
   
如下载
https://www.bilibili.com/video/BV1154y167zA?p=2
参考 https://blog.csdn.net/COCO56/article/details/106739521
3.3. 下载一个系列的所有视频
如果需要把这些视频全部下载，则需要在后面添加--playlist，例如：
you-get https://www.bilibili.com/video/BV1154y167zA --playlist
--->BV1154y167zA   这个是视频号 可根据自己的配置

****************分隔符****************
这里我选择下载了两个文件都是能正常下载的，
如果需要多个文件下载，请按照格式添加修改video后面的BV号即可；
想写python实现下载了。在研究xpath解析。
就这样干饭。you！get？


