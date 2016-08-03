# Better Mac

推荐 macOS 平台下的优秀应用、插件、技巧等。 

更多：[Better 系列](./README.md)

#### 评分说明

| 评分 |★★★★★ | ★★★★☆ | ★★★★ |★★★☆ |★★★   |
| --- | ---  | --- | --- | --- | --- |
| 说明 | 强烈推荐  | 十分优秀 | 值得使用 | 亮点突出 | 同类出众 |


## 应用

#### 效率工具

| 评分 | 名称 | 简介 | 价格 | 评测 |
| --- | --- | --- | --- | --- |
| ★★★★★ | [Alfred][alfred] | 超越 Spotlight | [£17、£27、£32][alfred-price] | # |
| ★★★★★ | [PopClip][popclip] | 文字选中弹出 Menu 扩展 | $6.99 | # |
| ★★★★★ | [iStat Menus][istatmenus]| 实时显示系统状态、网速等 | $18、$25 | # |
| ★★★★★| [Bartender][bartender] | 管理 Menubar 图标 | [$15][bartender-price] | # |
| ★★★★☆ | [Moom][moom] | 窗口管理切换工具 | [$10][moom-price] | # |
| ★★★★☆ | [1Password][1password] | 密码管理 | [$5/Mon、$64.99][1password-price] | # |
|  |  |  |  | 待续... |

[alfred]: https://www.alfredapp.com/
[alfred-price]: https://www.alfredapp.com/powerpack/buy/
[popclip]: http://pilotmoon.com/popclip/
[istatmenus]: https://bjango.com/mac/istatmenus/
[bartender]: https://www.macbartender.com/
[bartender-price]: http://sites.fastspring.com/macbartender/product/buybartender2
[moom]: https://manytricks.com/moom/
[moom-price]: https://sites.fastspring.com/manytricks/instant/moom
[1password]: https://1password.com/
[1password-price]: https://1password.com/pricing/


#### 开发

| 评分 | 名称 | 简介 | 价格 | 评测 |
| --- | --- | --- | --- | --- |
| ★★★★★ | [Sublime Text][sublime] | 编辑器 | [$70.00][sublime-price] | # |
| ★★★★★ | [iTerm][iterm] | 更好用的终端 | 免费 | # |
| ★★★★★ | [Tower][tower] | Git 客户端 | [$39.50、$79.00][tower-price] | # |
| ★★★★☆ | [MacVim][macvim] | Vim 编辑器 | 免费 | # |
|  |  |  |  | 待续... |


[sublime]: https://www.sublimetext.com/
[sublime-price]: https://www.sublimetext.com/buy
[iterm]: https://www.iterm2.com/
[tower]: https://www.git-tower.com/buy
[tower-price]: https://www.git-tower.com/
[macvim]: http://macvim-dev.github.io/macvim/



## Tips

#### 开机启动
添加应用程序到开机启动：“System Preferences” - “Users & Groups”（左下角）- “Login Items”。

#### 网络共享
开启 Wi-Fi 共享：“System Preferences” - “Sharing” - 左侧勾选 “Internet Sharing”，右则选择 “以太网” (Ethernet)，勾选 WiFi。

点击 “Wi-Fi Options” 选择 WPA2 可以设置密码。

#### 显示、隐藏不可见文件
macOS 系统把以 `.` 开头命名的文件视为不可见文件，正常情况下是隐藏的，如 `.DS_Store` 和 `.gitignore`。

```bash
#【显示】不可见文件
defaults write com.apple.finder AppleShowAllFiles -bool true
killall Finder

#【隐藏】不可见文件
defaults write com.apple.finder AppleShowAllFiles -bool false
killall Finder
```




## 候选名单
#### 常用目录
- 应用数据：~/Library/Application Support

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