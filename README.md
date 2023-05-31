# wordflows\_flutter\_jobs
笔试题。有问题可以在这里评论 或者邮件我。

文件如果在线不能查看的话，建议：
- 检查翻墙是否生效
- git clone，这个好像是不需要翻墙的
- 分支里有其他题目(除了main)

你好，感谢你的时间!

## 题目介绍
视频播放，并显示字幕，以及高亮字幕中给定的单词。

### 要求
1. 必须使用 Flutter
2. 可以使用任意插件; 可以使用任何开源代码

### 功能
wordflows.json 是需要显示出来的数据。以wordflows.json的结构来讲解
1. 将这个视频播放出来，显示在屏幕中间。 
- wordflows.json#video#url
2. 在视频播放的同时，跟随视频播放的进度，显示字幕。字幕显示在屏幕底部。(效果图 I’ll be happy to reimburese xxx 的部分)。这个案例中，有两个字幕，都需要显示出来。从上到下排列，文字居中。
- wordflows.json#subtitles[0][‘lines’]
- wordflows.json#subtitles[1][‘lines’] 
3. 在屏幕顶部显示单词。 wordflows.json#words[0] 这个案例中，只有一个单词。
4. 在字幕中高亮单词。正如效果图中 “I’ll be happy to reimburese xxx” 这句字幕的 ‘reimburese’ 是高亮的。需要高亮的词是: 
- wordflows.json#highlightWords[0][‘subWords’][0] 
- wordflows.json#highlightWords[0][‘subWords’][1]
- 显示圆形头像。如效果图中竖向居中，靠右显示的那个
- wordflows.json#user#smallAvatar

### 你不需要关注的部分
1. 底部的4个按钮。由于没有切图，你无法实现，但是你也可以用近似的素材替代。 
2. 顶部的导航条。使用Placeholder占位，或一个近似效果。
3. 右上⻆的头像。使用Placeholder占位，或一个近似效果。
### 其他
再次感谢你的时间，如果你的时间不充裕，或部分效果有难度，那么可以使用替代效果，或者部分不实现，能做多少是多少。但**代码需要能够在真机运行，没有闪退**。
### 面试
请将以上项目结果发到:
1. jianhua(AT)qqss.tech
2. 可以是zip包，但是更建议是github的仓库地址
3. 邮件中说明你的联系方式和简历。我们将通知面试。

### 效果图.jpeg
效果图

### wordflows.json
要用到的数据

### sample1.mp4
最终效果视频示例
###  sample2.mp4
最终效果视频示例

## 其他题目
切换分支：
- master: 播放和视频和显示字幕。主要用到状态管理，可以使用Provider来写逻辑，或使用其他方法。
- choice: 单词选择。主要用到手势和动画。
