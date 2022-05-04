# 0. 使用教程
[由此开始 - Obsidian 中文帮助 - Obsidian Publish](https://publish.obsidian.md/help-zh/%E7%94%B1%E6%AD%A4%E5%BC%80%E5%A7%8B)


[[Obs#1] 超強筆記軟體Obsidian (黑曜石)介紹教學與Zettelkasten筆記系統簡述 (CC字幕)_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV14v41137ip?spm_id_from=333.999.0.0)

[Johnny学的公开课 第一集 将近3小时的Obsidian小白入门课，都是基础 - 哔哩哔哩 (bilibili.com)](https://www.bilibili.com/read/cv13976033?spm_id_from=333.999.0.0)


# 1. Obsidian简介
## obsidian 特点
1. 支持markdown
2. 双链笔记
3. 插件丰富
4. 自定义模版
5. 内容纯文本。脱离工具，导入导出方便
6. 完全**本地保存**
7. 完全透明

## 知识管理流程
1. 学习知识
2. **保存知识**（笔记的作用）
	1. 输出，可以使用markdown
	2. 整理，可以使用双链
3. 使用知识
4. 共享知识
5. 创新知识

## 其他
1. 个人完全免费，商用付费
2. 收费功能：官方同步收费，但可以通过icloud等第三方工具实现。发布收费，但也用不上。


# 2. 认识Obsidian
## 资料库(vault)
obsidian 的所有内容都是基于资料库，后续的链接、图谱等功能都要基于同一个资料库，不能从A资料库链接到B资料库。所以创建资料库时，要想清楚这个资料库的定位是什么。

当创建好一个资料库后，所有关于这个资料库的设置，都会保存在这个资料库的`.obsidian`文件夹中。下面是一个库存储结构：
```bash 
demo
├── .obsidian
│   ├── .DS_Store
│   ├── app.json
│   ├── appearance.json
│   ├── backlink.json
│   ├── core-plugins.json   // 插件
│   ├── graph.json
│   ├── hotkeys.json        // 快捷键
│   ├── snippets
│   ├── themes              // 主题
│   │   ├── Blue Topaz.css
│   │   └── Minimal.css
│   └── workspace
├── .trash
│   └── 软件使用.md
├── attachments
│   └── Pasted image 20220429151150.png
├── docker
├── 软件使用
│   ├── attachments
│   │   ├── image-20220429004207106.png
│   │   └── image-20220429005537603.png
│   ├── obsidian 使用.md
│   └── 笔记软件对比.md
└── 笔记规范.md
```

当切换到一个新库时，会发现所有之前的设置（包括主题、快捷键、插件）都没有了。这是可以将`.obsidian` 文件夹复制过去。

## 界面
![[attachments/Pasted image 20220430164620.png]]
- 面板区可以根据不同设置，展示出不同面板

## 编辑
**对文件的编辑最好都在Obsidian中进行**，如果一个库中有了链接，直接编辑文档可能导致ob识别不到。

## 重要设置
### 文件与链接
- 删除移到`.trash`文件夹
- 新建笔记的存放位置
- 新附件的存放位置
![[attachments/Pasted image 20220502184920.png]]


## 核心插件
部分插件在**左侧或右侧功能区**显示。部分在展示区**右上角三个点**点开可以看到效果。

- 模版
通过模版直接生成文件的

- 标签面板
语法：类似一级标题，但不要空格就行。打开后在右侧会出现一个标签面板

- 幻灯片
通过分割线，可以实现幻灯片展示

- 工作区
打开后可以保存当前工作区的布局


# 3. 双链
[【课时4 双链的用法和价值】顶级知识管理神器、双链笔记先驱](https://www.bilibili.com/video/BV1yq4y1e7UB/?spm_id_from=333.788)

## 什么是双向链接
双向链接包括两个：出链（反向链接）、入链。
举个例子：A文件中引入了B，则A有一个出链，B有一个入链


## 使用双链
[嵌入文件 - Obsidian 中文帮助 - Obsidian Publish](https://publish.obsidian.md/help-zh/%E4%BD%BF%E7%94%A8%E6%8C%87%E5%8D%97/%E5%B5%8C%E5%85%A5%E6%96%87%E4%BB%B6)
可以嵌入图片，pdf，视屏，音频。安装插件后，可以给视频音频打上时间戳。

## 双链和普通 markdown 链接的区别
- 差异
	- 双链不是基本的markdown语法，普通的 markdown 编辑器无法正确解析。
	- 普通链接无法在关系图谱中显示关联。
- 相同
	- ob中，普通链接和双链在改文件名的时候，都会提示你是否要更改链接的文件。
	- ob中，删除附件（文件）时，都会提示你这个附件（文件）正在使用。


# 4. 使用技巧
## 模版功能
设置模版的文件夹，通过模版直接生成笔记。一般在库下单独设置一个文件夹 `template` 
来存放所有模版。


## 日记（特例的模版功能）
可以通过帮助文档提供的语法，设置文件名格式。


## 快捷键
- 分栏打开笔记：按住cmd点开文件
- 编辑模式预览链接：按住cmd同时将鼠标悬停在链接上
- 标题上右键，可以移动章节到别的文件。
- 右侧大纲中拖动章节，可以排列章节顺序，但不能自动调节章节的级别

# 5. 第三方插件

## 功能增强
- 自动维护附件的插件
[自动维护Markdown相容性的外掛：obsidian-consistent-attachments-and-links](https://www.bilibili.com/video/BV1oT4y1y7oH?spm_id_from=333.337.search-card.all.click)

- `File Explorer Count` 显示文件夹下笔记数量
- `Recent Files`  显示最近打开的笔记
- `obsidian-git` 通过github同步ob库
- `Pane Releif` 快速跳转当前面板前后打开过的笔记
- `Remember cursor position` 下次打开一个文件时，光标放在上次关闭时的位置

## 编辑
- `cMenu` 将常见格式显示成选项条
- `Hover Editor` 浮動式編輯窗格
- `Admonitions`
## 视觉效果
- `Minimal Theme Settings` + `Style Settings`，设置Minimal主题

## 其他工具
- `Obsidian exporter` 将储存库导出成标准Markdown格式，这个不是插件。






