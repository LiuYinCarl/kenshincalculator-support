# kenshincalculator-support

简洁计算器（KenshinCalculator）的静态技术支持站，用 GitHub Pages 托管。
无构建步骤、无 JavaScript，纯静态 HTML/CSS。

- **技术支持页：** https://liuyincarl.github.io/kenshincalculator-support/ ——填入 App Store Connect 的「技术支持网址」
- **隐私政策：** https://liuyincarl.github.io/kenshincalculator-support/privacy.html ——填入「隐私政策网址」（独立字段，不能与技术支持页互为同一 URL）

## 文件

- `index.html` ——技术支持页
- `privacy.html` ——隐私政策
- `styles.css` ——共用样式（`prefers-color-scheme` 自适应浅色/深色；accent 取自 App 等号键琥珀色）
- `assets/icon.png` ——App 图标，取 App 工程 `AppIcon.appiconset` 的 1024 图缩到 256

推送到 `main` 后自动重新部署（通常一分钟内生效）。

## 支持渠道

支持邮箱：kenshinliu@126.com（两个页面的唯一联系方式，不用 GitHub Issues）。
为保持 App Store 链接有效，**本仓库必须保持公开**。

## 口径纪律

隐私政策里的每一句都要对应 App 代码的真实行为（当前口径：完全离线、不收集数据、
无第三方 SDK、无权限申请、无内购）。**改 App 的联网 / 存储 / 权限 / 内购行为时，
同一个提交回来改本站对应页面。** 提审前逐条核对：技术支持 URL、隐私政策 URL、
App Store「App 隐私」标签三者一致。

## 改图标 / 版本号

- App 发新版本后，把 `index.html` 里 chips 中的版本号同步更新；
- 图标更换后重新从 `AppIcon.appiconset/icon_1024.png` 缩一份 256 的覆盖 `assets/icon.png`
  （`sips -z 256 256 icon_1024.png --out assets/icon.png`）。
