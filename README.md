# 北科大通識

## Youtube Download

### Step1. 找到隱藏網址

F12(開發人員工具) -> Network(上方TAB) -> XHR(中間TAB) ->找到有videoplayback字樣

![](https://github.com/Elwing-Chou/tt/raw/master/yt.png)

從content-type確定是video還是audio

接著把網址的 &range=0-95844 去掉, 就得到整段影片/聲音

### Step2.轉換檔案

[下載ffmpeg(Windows)](https://ffmpeg.zeranoe.com/builds/macos64/static/ffmpeg-20191203-12bbfc4-macos64-static.zip)

[下載ffmpeg(MAC)](https://evermeet.cx/ffmpeg/ffmpeg-4.2.1.7z)

打開電腦的終端機, 下指令

> 只想要聲音: XXXXX/XXXX/ffmpeg.exe(用拖的) -i xxx/weba(聲音位置) out.mp3(輸出檔名)

> 合併: XXXXX/XXXX/ffmpeg.exe(用拖的) -i xxx/weba(聲音位置) -i xxx/webm(影片位置) out.mp3(輸出檔名)
