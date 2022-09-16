# 将摄像头采集的数据存成YUV文件 
### 作者：张瀚文 2201212865
### 要求：
- 帧率 : 15fps
- 尺寸 : 320x2440
- 色度格式 : 4:2:0
### 步骤：
1. 下载ffmpeg格式转换工具 https://ffmpeg.org/about.html
2. 在ffmpeg目录下打开终端，并把需要转换格式的视频存储在这个目录下方便操作，命名为yami.mp4
![](https://github.com/hanwen76/DMT_2022/blob/main/camera2YUV/preparation.png)
3. 在终端输入视频格式转换的指令
```./ffmpeg -i yami.mp4 -s 320x240 -pix_fmt yuv420p -r 15 yami.yuv```
4. 运行指令，可以观察到目录下新生成的yami.yuv文件
![](https://github.com/hanwen76/DMT_2022/blob/main/camera2YUV/runPowershell.png)
![](https://github.com/hanwen76/DMT_2022/blob/main/camera2YUV/generateYUV.png)
5. 下载YUView，播放YUV格式的视频，检验格式是否转换成功;播放时注意设置好尺寸和色度格式
![](https://github.com/hanwen76/DMT_2022/blob/main/camera2YUV/viewYUV.png)
