# Atrium Nav · 玻璃拟态网址导航

![screenshot](docs/screenshot.png)

一个**单文件**的液态玻璃（Liquid Glass）风格浏览器起始页 / 网址导航页 —— `index.html` 一个文件装下全部逻辑，双击即用，无需安装、无需后端。

> 本项目的设计灵感与部分代码来自 [wynter-yaxley/atrium-desktop](https://github.com/wynter-yaxley/atrium-desktop)（C# 桌面玻璃美化项目），在此向原作者致谢 🙏 —— 本仓库将其玻璃视觉语言移植成了纯 Web 实现，并做了大量导航场景的适配。

## ✨ 功能

- **玻璃搜索框**：可切换/自定义搜索引擎（百度 / Bing / Google / 搜狗 / 360 / 哔哩哔哩内置）
- **搜索历史**：最多 9 条，支持单条删除、暂停与清空
- **直达网站**：快捷入口行，可自由增删（默认 DeepSeek）
- **百度热搜**：实时滚动热榜，悬停放大，明暗主题自适应
- **网址导航面板**：分组管理、跨分组移动、批量编辑、单条 Logo 自定义（自动抓取 favicon / 上传图片 / 首字兜底）
- **一键导入浏览器收藏夹**：支持 Chrome / Edge 的 `Bookmarks` 文件与导出的 `bookmarks.html`，自动识别浏览器并给出文件路径
- **任务栏**：访问量 Top-N 图标（数量可调）、悬停波浪放大（倍数可调）、音量/网络信号托盘图标（可开关）
- **时钟与天气**：秒级时钟 + 实时天气（Open-Meteo，自动定位，多源兜底）
- **缩放**：右上角 ±5% 缩放，支持自由输入（50–200%）
- **壁纸**：内置 4 张液态玻璃壁纸，支持纯色（HEX 直输 + 系统调色板）、上传图片、拖拽/粘贴
- **明暗自适应**：根据壁纸亮度自动切换文字主题
- **配置迁移**：一键导出/导入 JSON 配置，跨电脑迁移无忧

## 🚀 使用

```bash
git clone https://github.com/<owner>/atrium-nav.git
# 然后直接双击 index.html，或
cd atrium-nav && python -m http.server 8000
```

浏览器打开后：左下角九点按钮悬停呼出网址导航 → 右上角笔形图标进入批量编辑 → 添加网址或一键导入收藏夹。

## 📦 环境要求

无。任何现代浏览器（Chrome / Edge / Firefox）直接打开即可。

> 注：天气、热搜需要联网；`file://` 直开时部分外部请求可能被浏览器 CORS 策略拦截，用本地静态服务打开体验最佳。

## 🧩 结构

```
atrium-nav/
├── index.html          # 全部逻辑（HTML + CSS + JS 单文件）
├── wallpapers/         # 内置壁纸
└── docs/screenshot.png # 预览图
```

## 🙏 致谢

- [wynter-yaxley/atrium-desktop](https://github.com/wynter-yaxley/atrium-desktop) —— 本项目的玻璃设计语言、任务栏波浪交互动效与部分实现思路源自该项目，特此感谢！
- 视觉灵感来自 Apple Liquid Glass；本项目与 Apple、Microsoft 无关。

## 📄 License

[MIT](LICENSE) © 原作者 [wynter-yaxley](https://github.com/wynter-yaxley) 及本仓库贡献者。
