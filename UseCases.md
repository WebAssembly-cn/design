# 使用场景

WebAssembly 的[整体目标](HighLevelGoals.md) 定义了 WebAssembly 适合做*什么*。那些事在 Web 平台可以实现的，那些是非 Web 平台可以实现的。下面给出了一个不完善的无序列表，包括应用/领域/计算等方向，它们可能将从 WebAssembly 中受益的， WebAssamlby 的设计过程中也会将它们做为用例。

## 在浏览器中

* 更好的让一些语言和工具可以编译到 Web 平台运行。
* 图片/视频编辑。
* 游戏：
  - 需要快速打开的小游戏
  - AAA 级，资源量很大的游戏。
  - 游戏门户（代理/原创游戏平台）
* P2P 应用（游戏，实时合作编辑）
* 音乐播放器（流媒体，缓存）
* 图像识别
* 视频直播
* VR 和虚拟现实
* CAD 软件
* 科学可视化和仿真
* 互动教育软件和新闻文章。
* 模拟/仿真平台(ARC, DOSBox, QEMU, MAME, …)。
* 语言编译器/虚拟机。
* POSIX用户空间环境，允许移植现有的POSIX应用程序。
* 开发者工具（编辑器，编译器，调试器...）
* 远程桌面。
* VPN。
* 加密工具。
* 本地 Web 服务器。
* Common NPAPI users, within the web's security model and APIs.（没懂）
* 企业软件功能性客户端（比如：数据库）


# 脱离浏览器

* 游戏分发服务（便携、安全）。
* 服务端执行不可信任的代码。
* 服务端应用。
* 移动混合原生应用。
* 多节点对称计算


# 如何使用 WebAssembly

* 整个代码库都用 WebAssembly。
* 主要使用 WebAssembly 计算，UI 使用 JavaScript/HTML。
* 在大型 JavaScript/HTML 应用中复用已经存在的 WebAssembly 代码。像使用助手库一样，分担一些计算任务。