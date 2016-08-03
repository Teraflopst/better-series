# Better Alfred

推荐实用的 Aflred 技巧和 workflow。

更多：[Better 系列](./README.md)

我的：[Alfred Workflow](https://github.com/onestark/alfred-workflows)

#### 评分说明

| 评分 |★★★★★ | ★★★★☆ | ★★★★ |★★★☆ |★★★   |
| --- | ---  | --- | --- | --- | --- |
| 说明 | 强烈推荐  | 十分优秀 | 值得使用 | 亮点突出 | 同类出众 |

## Workflow
### 1. Workflow 推荐列表
更多 workflow 请访问 [alfredworkflow.com](http://alfredworkflow.com/) 和 [packal.org](http://www.packal.org/)

| 评分 | 名称 | 简介 | 类型 | 说明 |
| --- | --- | --- | --- | --- |
| ★★★★ | [Packal Workflow Search] | 在 Packal.org 查找 workflow |  工具| 使用 Packal.org 管理 workflow |
| ★★★★ | [Packal Updater] | 从 Packal.org 更新 workflow | 工具 | 使用 Packal.org 管理 workflow |
| ★★★★ | [TinyPNG] | 压缩图片 | 图像 | 调用 TinyPNG API 压缩图片<br>API 限制每月免费 500 张 |
| ★★★★ | [有道翻译][youdao] | 词典、翻译 | 工具 | 支持直接发音 |
| ★★★★ | [Chrome Bookmarks] | 搜索 Chrome 书签 | 效率 | 比地址栏搜索书签更准确 |
| ★★★★ | [Open with][Open Sublime]<br>[Sublime Text][Open Sublime] | 快速使用 Sublime Text 打开文件 | 效率 | 配合快捷键使用效率大增<br>附：[Open with...] 系列 |
| ★★★★ | [百度 CDN] | 快速获取百度静态资源公共库链接 | 效率/开发 | [百度静态资源公共库](http://cdn.code.baidu.com/) |
| ★★★☆ | [Dash] | 快速搜索开发文档，开发者必备 | 效率/开发 | 需要配合 [Dash 应用]使用 |
| ★★★☆ | [caniuse] | [Can I use](http://caniuse.com/) 快速查找 | 效率/开发 | 前端兼容性问题必备利器 |
| ★★★☆ | [Lorem Ipsum] | 生成乱数假文 | 效率/工具 | Lorem ipsum dolor sit... |
|  |  |  |  | 待续... |


[Chrome Bookmarks]:https://github.com/blainesch/alfred-chrome-bookmarks

[Packal Workflow Search]: http://www.packal.org/workflow/packal-workflow-search

[Packal Updater]: http://www.packal.org/workflow/packal-updater

[TinyPNG]: http://www.packal.org/workflow/tinypng
[youdao]: https://github.com/liszd/whyliam.workflows.youdao

[Chrome Bookmarks]: https://github.com/blainesch/alfred-chrome-bookmarks

[Open Sublime]: https://github.com/franzheidl/alfred-workflows/
[Open with...]: https://github.com/franzheidl/alfred-workflows/
[Dash]: https://github.com/Kapeli/Dash-Alfred-Workflow
[Dash 应用]: https://kapeli.com/dash
[caniuse]: https://github.com/willfarrell/alfred-caniuse-workflow
[百度 CDN]: https://github.com/onestark/alfred-workflows
[Lorem Ipsum]: http://jgpippin.com/2014/04/alfred-workflow-lorem-ipsum/

### 2. Workflow 资源集合

- [franzheidl/alfred-workflows](https://github.com/franzheidl/alfred-workflows)
- [willfarrell/alfred-workflows](https://github.com/willfarrell/alfred-workflows)（for 开发者）
- [onestark/alfred-workflows](https://github.com/onestark/alfred-workflows)（我的）



## 技巧
Spotlight

### 0. 备份
Alfred 最重要的一点是备份数据。（延伸到任何有价值的数据...）

**Alfred Preferences - Advanced** 右下角中选择备份的路径。

### 1. 搜索
Alfred 提供多种搜索模式，官方最推荐的是使用 Quick Search，即调出搜索栏后，按下空格键 `Space` 或单引号 `'`。选择候选结果直接按下 `↩` 使用默认程序打开文件；按下修饰键 `⌘` + `↩` 在 Finder 中显示文件。

可以设置前缀的另外几种模式：

- 搜索并打开文件（和按下空格键是相同的）
- 搜索并在 Finder 显示文件
- 搜索文件中的内容
- 搜索 tags

#### 系统文件
Alfred 的文件搜索是默认不能搜索系统文件的。

例如，macOS 通常会把在 `~/Library` 文件夹中的文件当作系统文件，标记为 `MDSystemFile`，对 Alfred 和 Spotlight 的搜索都是不可见的。

**解决**：在一个 workflow 的 `File Filter` 中，**Search Scope** 选项可添加搜索范围，勾选 *Show files marked as System File* 即可搜索到范围内的系统文件。

**注意**：太多的系统文件会导致太多的搜索结果，对搜索结果造成干扰。

### 2. 文件操作

Alfred 提供了类似右键菜单的功能 **File Action**，可以选择文件后使用快捷键触发，也可以在 Alfred 的文件搜索结果中按下方向右键触发。菜单功能包括常见的文件复制、移动、删除等，此外，在 workflow 中添加 `File Action` 入口也可以扩展文件动作菜单。

另外，File Action 菜单右侧有预览小窗口。

#### Buffer
把多个文件添加到 buffer，可以实现批量处理。我们平时使用鼠标或键盘来多选多个文件，然后右键呼出菜单来完成多文件的操作，这局限于在同一个文件夹中的文件。Alfred 的 buffer 功能可以实现不同文件夹文件的批量操作：

1. 使用 Alfred 搜索并选中文件；
2. 按下右方向键 `➝` 呼出动作菜单；
3. 按下 `⌥` + `↑` 添加文件到 buffer 中；
4. 按下 `⌥` + `→` 呼出多文件动作菜单。


`⌥` + `←` 把文件逐个移出 buffer

`⌥` + `↓` 同样是添加文件到 buffer 中，不同的是选区会同时移到下一项

另，在 buffer 中的文件会在搜索栏左上角显示小图标。

#### 预览
使用 Alfred 搜索文件，在候选结果列表中选择文件，按下 `⇧`（Shift）可以调用 macOS 的预览（Preview）功能。或 `⌘` + `Y`。







## 关于

#### 评分说明：

| 评分  | 推荐度 | 说明 | 解释 |
| ---  | --- | --- | --- |
|★★★★★ | 5.0 星 | 强烈推荐 | 极大地提高了效率或扩展了系统功能，推荐必装必用 |
|★★★★☆ | 4.5 星 | 十分优秀 | 在特定领域十分优秀，具有针对性和专业性的推荐 |
|★★★★  | 4.0 星 | 值得使用 | 在特定领域值得使用，具有针对性和专业性的推荐 |
|★★★☆  | 3.5 星 | 亮点突出 | 亮点鲜明，解决需求；可能不常用，但很好用 |
|★★★   | 3.0 星 | 同类出众 | 同类中值得关注和试用 |

#### 注意事项：
1. 此列表排名分先后
2. 此列表含有个人主观
