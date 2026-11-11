# clash verge ios：有 iPhone 版吗？

查找 clash verge ios，可以直接得到答案：写这一页时(2026-11-08)，Clash Verge 与 Clash Verge Rev 都没有 iOS 版本，支持的平台是 Windows、macOS 和 Linux。想在 iPhone 上使用 Clash 配置，可以查看 Stash、Karing 对配置兼容性的说明；它们是独立客户端，不是 Clash Verge 的手机版。

## 为什么找不到 iOS 版？

先核对项目支持的平台。[Clash Verge Rev 仓库](https://github.com/clash-verge-rev/clash-verge-rev)的介绍面向桌面系统，README 列出的支持范围也只有上述三类系统，没有列出 iOS。

再看项目实际提供的安装文件。写这一页时(2026-11-08)，[发布页](https://github.com/clash-verge-rev/clash-verge-rev/releases/tag/v2.5.10)中的安装文件分别用于 Windows、macOS 和 Linux，没有供 iPhone 安装的包。这与仓库介绍、README 的平台范围一致。

移动端计划也有明确答复。写这一页时(2026-11-08)，可查到维护者在移动端请求议题中表示不考虑，解释涉及部分 Rust、Node.js 依赖难以迁往移动设备。这是当时的项目答复，不能据此推断以后永远不会改变。

## Clash Verge 和 Rev 怎么区分？

核对名称时，也要看仓库所属项目。写这一页时(2026-11-08)，原版 zzzgydi/clash-verge 已归档，Clash Verge Rev 则仍在维护，仓库没有归档，当日还有提交记录。两者面向的都是桌面系统。

“Rev 仍在维护”与“有 iPhone 版”是两回事。判断能否用于手机，要看支持平台和发布文件，不能只凭项目名称或维护状态作判断。

> [!NOTE]
> 遇到带有 Clash Verge 名称的 iOS 安装信息，先回到项目发布页核对。名称相同，不能证明文件由该项目发布。

## iPhone 上哪些客户端说明支持 Clash 配置？

先看配置兼容范围，再核对手机系统要求。下面两款都有自身文档或仓库说明，可以据此区分支持内容。

写这一页时(2026-11-08)，对应的系统要求及美区商店收费信息如下：

| 客户端 | 对 Clash 配置的说明 | 系统要求 | 美区商店 |
| --- | --- | --- | --- |
| Stash | 文档说明其内核兼容 Clash 配置标准 | iOS 16.0 起 | 付费 |
| Karing | README 说明支持 Clash 配置，对 clash.meta 配置为部分支持 | iOS 15.0 起 | 免费 |

[Stash 文档](https://stash.wiki/)说明了配置标准的兼容关系。[Karing 仓库](https://github.com/KaringX/karing)则区分了 Clash 与 clash.meta 的支持程度。要沿用已有配置，应留意这一区别，不能把“部分支持”理解为所有内容都能直接使用。

写这一页时(2026-11-08)，中国区 App Store 查询没有返回这两款应用。查询为空可能与地区供应范围或查询方式有关，不能直接认定应用已经下架。

## 常见问题

### iPhone 能安装 Clash Verge Rev 吗？

写这一页时(2026-11-08)，项目没有提供 iOS 版本，现有发布文件用于桌面系统。判断手机能否安装，应核对项目发布页列出的平台，不能把桌面安装文件当作手机安装包。

### Stash、Karing 是 Clash Verge 的手机版吗？

它们是各自独立的客户端。两者的说明涉及读取 Clash 配置的能力，这与 Clash Verge 是否发布手机版是不同问题。选择时应分别核对应用名称、配置支持范围和系统要求。

### 支持 Clash 配置，就代表全部兼容吗？

不能仅凭“支持”二字作这样的判断。Karing 明确区分了 Clash 配置与 clash.meta 配置的支持程度；Stash 则说明了自身兼容的配置标准。应以各自说明的具体范围为依据。
