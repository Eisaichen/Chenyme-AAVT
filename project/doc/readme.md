<div align="center">
  
# AI Auto Video(Audio) Translation 


[![简体中文 badge](https://img.shields.io/badge/%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87-Simplified%20Chinese-blue)](./README.md)
[![英文 badge](https://img.shields.io/badge/%E8%8B%B1%E6%96%87-English-blue)](./README-EN.md)
[![下载 Download](https://img.shields.io/github/downloads/Chenyme/Chenyme-AAVT/total.svg?style=flat-square)](https://github.com/Chenyme/Chenyme-AAVT/releases)
![PyPI - Version](https://img.shields.io/pypi/v/AAVT)

Chenyme-AAVT V0.8.3
</div>


非常感谢您来到我的 **全自动视频翻译** 项目！该项目旨在提供一个简单易用的全自动视频（音频）识别、翻译工具，帮助您快速识别视频字幕并翻译生成字幕文件，然后将翻译后的字幕与原视频合并，以便您快速的实现视频翻译。


> - **Note ：字幕翻译的错位问题会逐步优化。由于考研，更新速度可能会放缓，感谢理解~~~**
> - **Tips1 ：推荐选用 Faster-whisper 和 Large 模型以获得最好的断句、识别体验。**
> - **Tips2 ：新版本改动很大，BUG较多，因此近期更新比较频繁，建议更新。**
> - **Tips3 ：这个版本以后更新不会这么勤了，学业为重，大家有问题可以加群讨论噢。**

#### 这次更新真的很耗时鸭！给一颗免费的星鼓励一下叭~感谢！[AAVT项目文档](https://zwho5v3j233.feishu.cn/wiki/OGcrwinzhi88MkkvEMVcLkDgnzc?from=from_copylink)

<table>
  <tr>
    <td><img src="https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/6641bdc9-02dc-437c-8cc1-160526da162e" /></td>
    <td><img src="https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/b20ddf3c-34c7-460b-bf98-fe66d856c6be" /></td>
  </tr>
</table>

#### [测试效果 点击下载](https://github.com/Chenyme/Chenyme-AAVT/blob/main/public/test_vedio.mp4?raw=true)

## 项目亮点
> *   支持 **OpenAI API 接口调用** 和 **Faster-Whisper 本地运行**。
> *   支持 **GPU 加速**、**VAD辅助**。
> *   支持 **ChatGPT**、**KIMI**、**DeepSeek**、**ChatGLM**、**本地部署模型** 多种翻译模式。
> *   支持 **调节多种参数**，满足定制化需求。
> *   支持识别、翻译 **多种语言** 和 **多种文件格式** 。
> *   支持 **一键生成** 处理好的内容。
> *   支持对 **字幕修改、微调、预览**。
> *   支持对内容直接进行 **AI总结、问答**。
> *   支持视频直接 **生成图文博客**。


## 如何安装

#### 1. 安装 [Python](https://www.python.org/downloads/)

- 请确保Python版本大于3.8

#### 2. 安装 [FFmpeg](https://www.ffmpeg.org/download.html)

- [**Release**](https://github.com/Chenyme/Chenyme-AAVT/releases) 中`Full`版本已经打包了FFmpeg库
 
- 设置 FFmpeg 环境变量
  
  - `Win+R` 快捷键打开运行对话框。
  - 输入 `rundll32 sysdm.cpl,EditEnvironmentVariables`。
  - 在用户变量中找到 `Path`。
  - 点击新建，输入 FFmpeg 的路径。 示例：`D:\APP\ffmpeg\bin`（请根据自己的实际路径调整）。

#### 3. 运行 `install.bat`

- 选择对应版本的 `install.bat`，等待安装所有依赖库
  
- CPU运行选择CPU版本，CUDA11.8、CUDA12.1同理

## TODO


### 识别相关
- [x] 更换更快的Whisper项目
- [x] 支持本地模型加载
- [x] 支持个人微调Whisper模型
- [x] VAD辅助优化
- [x] 字词级断句优化
- [x] 更多的语种识别

### 翻译相关
- [x] 翻译优化
- [x] 更多的语种翻译
- [x] 更多的翻译模型
- [x] 更多的翻译引擎
- [x] 支持本地大语言模型翻译

### 字幕相关
- [x] 个性化字幕
- [x] 更多字幕格式
- [x] 字幕预览、实时修改
- [ ] 自动化字幕文本校对
- [ ] 双字幕

### 其他
- [x] 视频总结、罗列重点
- [x] 视频预览
- [x] AI助手
- [x] 视频生成博客*
- [ ] 实时语音翻译
- [ ] 视频中文配音

##### 注：含`*`的功能还不稳定，可能存在某些BUG。

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Chenyme/Chenyme-AAVT&type=Timeline)](https://star-history.com/#Chenyme/Chenyme-AAVT&Timeline)

## 项目界面预览

### 主页面

![1716910190616](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/0bfebaf3-53c5-42ae-8031-b898dc27df6f)

### 设置

![1716910203660](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/49b89451-1129-4073-b1b5-0094af65f53e)

### 视频识别

##### 参数设置

![d967ac4074d0c8ecba07b95de533730](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/72bc0e88-2148-486c-ac46-4f87a55e946b)

##### 运行界面

![b861c5019833b770f98344f7a4c73a4](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/ced915ec-a07b-43d2-9cf9-f92910033cb9)

##### 视频生成

![1716650985701](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/04bdf745-7ece-4c8b-a97b-f779b632dbc3)

##### 字幕微调

![1716651009788](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/33a02ef5-7386-4f34-ba0b-8947f17b78e3)

### 内容助手

##### 参数设置

![461474f5d96b61b70bd239a9e3ddf8d](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/f22a11c2-3c58-4a92-ab4c-954e3710a254)

##### 运行界面

![14575fd5efbe138f364329626501b09](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/8a81ea44-95ae-488f-9412-014ff1c030e3)

### 字幕翻译

![35bc5a96676c7f2b9d71042eb7c877f](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/635865b1-6ec1-41fd-858c-e1dcc87d684b)


### 视频博客

![09f60b8099f8ce19b83f4da63b26817](https://github.com/Chenyme/Chenyme-AAVT/assets/118253778/bbfca353-53d4-4a19-994f-7beddbbf17d7)


## 鸣谢

#### 本人是 AI 时代的受益者，本项目的开发基本是站在巨人的肩膀上实现的。主要基于 OpenAI 开发的 Whisper 来识别声音和 LLMs 辅助翻译字幕 ，利用 Streamlit 搭建快速使用的 WebUI 界面，以及 FFmpeg 来实现字幕与视频的合并。
#### 非常感谢 OpenAI 、 Streamlit 、 FFmpeg 、Faster-whisper 等开发人员！


常见问题报告（FAQ）
1. 如何安装和配置AAVT项目？
回答：

安装依赖项：确保安装Python、Streamlit、Streamlit Antd Components、OpenAI、MoviePy、Faster Whisper和FFmpeg。
配置文件：编辑config/目录下的api.toml和video.toml文件，填入相应的API密钥和模型配置。
2. 支持哪些视频格式？
回答：

AAVT支持多种视频格式，包括mp4、mov、avi、m4v、webm、flv和ico等。
3. 如何选择识别和翻译模型？
回答：

在侧边栏的“识别设置”中，可以选择Whisper模式（OpenAI API接口调用或本地Faster Whisper模型）。
在“翻译设置”中，选择需要使用的翻译引擎（如ChatGPT、Kimi、ChatGLM、DeepSeek等），并设置原始语言和目标语言。
4. 为什么生成字幕时会出现RateLimitError错误？
回答：

这是由于API调用频率超过限制导致的。可以在“翻译设置”中适当增加翻译间隔（wait time），以减少API调用频率。
5. 如何解决GPU加速和CUDA问题？
回答：

确保系统已正确安装CUDA和Pytorch，并在配置文件中启用GPU加速。如果仍然无法使用GPU，可以检查CUDA和Pytorch的安装是否成功。
6. 如何处理本地模型加载问题？
回答：

确保本地模型文件已正确下载并存放在指定目录。在侧边栏的“识别设置”中选择本地模型加载模式，并指定正确的模型路径。
7. 生成字幕文件支持哪些格式？
回答：

AAVT支持生成多种字幕格式，包括SRT、ASS、STL和VTT等。
8. 如何查看和下载生成的字幕文件？
回答：

在生成字幕的过程中，生成的字幕文件会存放在指定的输出目录中。完成后，可以在侧边栏下载生成的字幕文件。
9. 为什么生成的视频无法预览？
回答：

可能是由于FFmpeg或CUDA状态异常导致的。请确保FFmpeg已正确安装，并检查CUDA状态。如果CUDA不可用，可以选择使用CPU模式生成视频。
10. 如何解决项目运行中的闪退问题？
回答：

可以查阅https://zwho5v3j233.feishu.cn/wiki/OGcrwinzhi88MkkvEMVcLkDgnzc?from=from_copylink或者在使用修复功能。如果问题仍未解决，请前往环境目录删除/Lib/site-packages/torch/lib/libiomp5md.dll文件。
如有其他问题，请查阅项目文档或联系项目维护者。