# XXP.AI — Selected Works

个人作品集主页。一个入口，三个可交互的作品——游戏能玩、地图能点、插件演示能切换步骤。

部署在 Cloudflare Pages，纯静态、无构建步骤、Git push 自动发布。

## 本地预览

```sh
python -m http.server 8000
```

打开 `http://localhost:8000`。不要直接双击 `index.html`（iframe 在 `file://` 协议下会被浏览器限制）。

## 目录结构

```
index.html                           主页：三个项目卡片，点击 LAUNCH 全屏运行
projects/
  stunt-racer/
    index.html                       赛车特技 · 单文件游戏本体（自包含）
    README.md                        玩法与设计说明
    docs/design-spec-v2.html         设计规格
    docs/mindmap.html                成果思维导图
  life-roaming-map/
    index.html                       人生漫游地图 · H5 体验版（源仓库 h5/index.html）
    README.md                        小程序与 H5 说明
  dsh-snip/
    index.html                       插件演示页（本仓库补充，源仓库无网页入口）
    README.md                        插件源码说明
    docs/overlay.png                 真实运行截图
```

## 三个项目

| 编号 | 项目 | 类型 | 展示方式 |
|---|---|---|---|
| 001 | DSH-SNIP | 工具 | 文档 + 分步高亮演示（Windows 桌面插件，无法在网页真运行） |
| 002 | 人生漫游地图 | 社交 | H5 完整可交互版，数据存浏览器本地 |
| 003 | 赛车特技 | 游戏 | 单文件游戏本体，键盘操作 |

## 同步源仓库

三个项目各有独立源仓库，本仓库只保留展示副本。源仓库更新后需手动同步：

```sh
curl --ssl-no-revoke -fsSL https://raw.githubusercontent.com/XXP-AI-SPACE/stunt-racer/main/index.html -o projects/stunt-racer/index.html
curl --ssl-no-revoke -fsSL https://raw.githubusercontent.com/XXP-AI-SPACE/life-roaming-map/main/h5/index.html -o projects/life-roaming-map/index.html
```

## 设计

赛博科幻 / 深空终端风格。底色 `#05080F`，信号色青 `#00E5C0`，字体 Space Grotesk + IBM Plex Mono。v0.1 原型，后续可迭代。
