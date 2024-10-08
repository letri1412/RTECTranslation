# RTECTranslation
_自用，RT社视频翻译流程参考_

**一、首先要挂上代理或VPN，不推荐Cloudflare美国相关节点**

**二、下载**

视频下载：https://savefrom.com.co/en211th/

视频下载备用：https://cobalt.tools/

如果视频无法直接下载视频，可以拆分成视频画面+视频音频下载

视频画面下载：https://savefrom.com.co/en211th/
视频音频下载：https://loader.to/

字幕下载：https://downsub.com

**三、字幕生成**

有时候某些视频没有字幕，就需要考虑自己生成字幕。

两种方法：云转录、本地转录

云转录可以使用网上的文本转语音功能，但大部分是要付费的。

本地转录可能会有错误，但是有较好的时间轴参考价值。

推荐使用开源项目Whisper借助大模型转录。

参考博主“零度解说”的文章：https://www.freedidi.com/8743.html

参考博主“零度解说”的视频：https://www.freedidi.com/8737.html

Whisper配置建议：
| 选项 | 建议 |
|---:|:---|
| 模型| 大型 |
| Language| Chinese |
| Translate| □ |
| 格式| SRT |

>如果转录出来的文本是繁体中文，可以用WPS Office的Word上方的“审阅”的“转简”功能。

>如果遇到了文本重复累赘的情况，可以把这段音频单独导出再用Whisper单独转录一次。

**四、剪辑**

前面要加片头，社区片头文件放[这里](https://github.com/letri1412/RTEDMIntros)了。

然后是视频开头的文本（宋体，左上角，左对齐，小字）：

```
RELECTECH电子音乐社区翻译组

翻译

审校

原作者

```

社区片头和翻译的视频之间最好加个转场（快捷键shift+d）

在视频中遇到了不符合法律法规的内容要去掉。

**五、字幕**

字幕轨道字体（只要是免费商用都可以）：鸿蒙字体 Medium、思源黑体CN Medium

字幕轨道中不可出现[music][音乐]这些字幕

关于嵌字，如果在翻译的视频内出现了博主自己的文本，自行斟酌是否要嵌字翻译。如果要，那一定要使用风格相似、字号相近、粗细相近的字体，并且有动画一定要尽可能还原，如故障效果和渐入渐出。

**六、翻译**

比较耗时间的步骤，需要检查翻译文本的正误，校准时间轴。

翻译文本时要确保语句通顺，可以适当加入梗相关的文本，以及其它更接地气的内容。

专业性的词语无法翻译时，可以使用英文，如果可以，最好在其它位置添加解释文本，但不能字幕轨道的阅读（不能遮挡，不能太大）

**七、审校**

既要检查字幕文本是否合适，又要检查字幕时间轴是否与音频对其，及时查漏补缺。

**八、导出**

视频画幅帧率与翻译的视频相同即可，目标比特率为2Mbps

音频参数，采样率44100Hz，比特率192kbps



---

此GitHub项目中的“RELECTECH电子音乐社区视频翻译.prproj”是Adobe Premiere Pro 2024的项目文件，不包含视频、字体、音频。
