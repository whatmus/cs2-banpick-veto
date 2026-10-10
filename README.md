# CS2 Ban & Pick

一个用于 Counter-Strike 2 比赛的轻量级地图禁选与播放页面。项目使用原生 HTML、CSS 和 JavaScript，无需构建工具或后端服务。

## 功能

- 设置 A、B 队名称，并上传自定义队伍图标。
- 从地图池中选择 3–7 张地图，可拖动或使用箭头调整顺序，并设置 BAN、PICK 或 DECIDER。
- 编辑地图显示名称，并为每张地图选择壁纸。
- 为 PICK 地图选择对手的 CT/T 开局阵营；为决胜图手动选择开局队伍和 CT/T 阵营。
- 在播放页面依次揭晓地图，可重播或一次显示全部地图。
- 设置保存在当前浏览器的本地存储中。

## 项目结构

```text
.
├── index.html              # 赛程编辑页面
├── display.html            # 地图播放页面
├── src/
│   ├── app.js              # 配置、交互和播放逻辑
│   └── style.css           # 页面样式
├── assets/
│   └── images/             # 地图壁纸、背景和 CT/T 图标
├── LICENSE                 # MIT 开源协议
└── README.md
```

## 本地运行

建议通过本地 HTTP 服务运行，以便浏览器正常读取图片资源：

```bash
python -m http.server 8000
```

然后在浏览器打开 [http://localhost:8000](http://localhost:8000)。也可以使用 VS Code Live Server 或其他静态文件服务器。

## 使用方法

1. 在 `index.html` 页面填写队伍名称并选择队伍图标。
2. 选择 3–7 张地图，设置流程、壁纸、名称和开局选边。
3. 点击“打开播放页面”进入 `display.html`，播放页会按顺序揭晓地图。

## 发布到 GitHub Pages

将仓库根目录作为 Pages 发布目录即可；入口文件是 `index.html`，播放页为 `display.html`。无需安装依赖或运行构建步骤。

## 开源协议

本项目采用 [MIT License](LICENSE) 开源。完整协议内容请参阅 `LICENSE` 文件。
MIT 协议适用于本项目代码；第三方项目及素材的权利仍归各自权利人所有，发布时请确认其使用和再分发条件。

## 致谢

- [SouthDream666/cs2-map-veto-overlay](https://github.com/SouthDream666/cs2-map-veto-overlay)
- TechSanjal 的 [valorant-map-veto-overlay](https://github.com/TechSanjal/valorant-map-veto-overlay)

本项目由 Codex 生成。

> 队伍名称、图标和赛程配置保存在访问者自己的浏览器中，不会自动同步到其他设备或浏览器。

---

# CS2 Ban & Pick

A lightweight map veto and presentation tool for Counter-Strike 2 matches. It is built with vanilla HTML, CSS, and JavaScript and requires no build tools or backend service.

## Features

- Set Team A and Team B names, and upload custom team logos.
- Select 3–7 maps, drag or use the arrow controls to reorder them, and assign BAN, PICK, or DECIDER roles.
- Edit map display names and choose a wallpaper for each map.
- Choose the opposing team’s CT/T starting side for PICK maps, and manually choose the starting team and side for the decider.
- Reveal maps in sequence, replay the presentation, or reveal all maps at once.
- Settings are saved in the current browser’s local storage.

## Project Structure

```text
.
├── index.html              # Match setup page
├── display.html            # Map presentation page
├── src/
│   ├── app.js              # Configuration and UI logic
│   └── style.css           # Page styles
├── assets/
│   └── images/             # Map art, background, and CT/T icons
├── LICENSE                 # MIT License
└── README.md
```

## Run Locally

Run a local HTTP server so the browser can load image assets reliably:

```bash
python -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in a browser. VS Code Live Server or any static file server also works.

## Usage

1. Enter team names and choose team logos on `index.html`.
2. Select 3–7 maps and configure roles, wallpapers, names, and starting sides.
3. Click **Open Presentation** on the setup page to launch `display.html` and reveal the maps in order.

## Deploy to GitHub Pages

Publish the repository root with GitHub Pages. The entry page is `index.html`, and the presentation page is `display.html`. No dependency installation or build step is required.

## License

This project is released under the [MIT License](LICENSE). See the `LICENSE` file for the full license text.
The MIT License applies to this project’s code. Third-party projects and assets remain subject to their respective rights and terms; verify their use and redistribution conditions before publishing.

## Acknowledgements

- [SouthDream666/cs2-map-veto-overlay](https://github.com/SouthDream666/cs2-map-veto-overlay)
- [valorant-map-veto-overlay](https://github.com/TechSanjal/valorant-map-veto-overlay) by TechSanjal

This project was generated with Codex.

> Team names, logos, and match settings are stored in each visitor’s browser and are not automatically shared across devices or browsers.
