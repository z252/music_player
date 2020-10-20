# music_player
## 说明
这是一个基于 MCI 播放，使用 easyx 作为界面的简单本地音乐播放器。

支持以下操作，设置音乐搜索路径（在文件中设置），播放，暂停，下一曲，上一曲，单曲循环，顺序播放（列表循环），随机播放，

设置音量大小，拖动音乐进度条（快进，快退），滚动条，展开/关闭播放列表，更换背景图等。

## 介绍
这是程序打开后的界面，此时播放列表默认为隐藏状态，鼠标点击播放列表或者其旁边的小箭头，即可展开音乐播放列表

![image1](f.myid.email/ca/de/42/320bb6-4309-a3ac-2b5efb21d7dc/Files/0x00.jpg)


下图为正在播放音乐时的界面，可以看到，有显示播放列表，右侧有播放列表的滚动条（紫色），显示音乐播放的进度条，

音乐名，音乐播放时间和音乐总时间等

点击播放列表中的音乐名即可播放该音乐，再次点击暂停

播放列表旁边的滚动条可上下拖动，也可以在其上下方位置点击移动（拖动操作可能体验较差，建议在其上下方点击）

音乐进度条可点击，拖动达到快进/快退操作（拖动操作暂时有着明显的延迟，顿挫感，建议进行点击操作）

同样，音量条可点击或拖动进行音量调节

暂停播放键可进行音乐的暂停播放

上一曲，下一曲根据播放模式的变化进行播放

播放模式，即图中的 随机播放 ，可进行点击切换播放模式，按照 单曲循环 -> 顺序播放 （列表循环）-> 随机播放 进行切换

右上角退出键，点击即可退出关闭音乐播放器

![image2](https://f.myid.email/ca/de/42/320bb6-4309-a3ac-2b5efb21d7dc/Files/0x01.jpg)


## 注意事项 
程序首次运行后会加载文件 filePath.ini 文件的内容，其中存放要进行搜索的路径名，若无该文件则程序会默认生成一个，

并将其写入 "." （当前路径）并设置当前搜索路径为 "."，请在首次运行前修改该文件，写入合适的音乐搜索路径。

搜索到的音乐文件完整路径名，将存放在文件 music.mn 中，如果程序检查到此文件存在将不会进行搜索操作，而只是读取该文件

所以，请在修改 filePath.ini 文件后删除此文件，下次运行程序后将读取 filePath.ini 文件配置，并进行搜索，

也可在此文件中进行音乐的删除，修改排列位置等操作。

若要修改背景图片，请将 background.jpg 图片替换，注意图片名称和格式需完全一致。
