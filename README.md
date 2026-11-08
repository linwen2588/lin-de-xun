# 林的训 PWA（本地保存版）

## 包含功能
- A/B 两套训练计划，预置当前训练动作，可自定义添加/删除动作
- 每组记录重量、次数；引体向上单独记录辅助重量
- 自动带入上次同动作的最后一组数据
- 组间休息倒计时，结束震动/提示（网页在后台时提醒可能受系统限制）
- 训练计时、历史记录、月训练次数/时长
- PR、体重/体脂/围度记录
- JSON 全量导入/导出备份
- PWA 安装配置与基础离线缓存

## 数据说明
数据仅保存在当前设备的当前浏览器 localStorage。手机和电脑各自有一份数据，不会自动同步。跨设备迁移请在一台设备导出 JSON，再在另一台设备导入。清除浏览器数据可能导致记录丢失，请定期备份。

## 发布到 GitHub Pages（免费）
1. 登录 https://github.com/ ，新建一个 Public repository，例如 `lin-de-xun`。
2. 解压本压缩包，把 `index.html`、`manifest.webmanifest`、`sw.js`、`icon.svg` 放在仓库根目录。
3. 在仓库打开 Settings → Pages。
4. 在 Build and deployment 中选择 Deploy from a branch；Branch 选 `main`，文件夹选 `/ (root)`，保存。
5. 等待发布完成，页面会给出网址，形式类似 `https://你的用户名.github.io/lin-de-xun/`。
6. 用安卓 Chrome 打开网址，菜单中选择“安装应用”或“添加到主屏幕”。
7. Windows Chrome/Edge 打开同一网址，选择地址栏安装图标，或菜单 → 保存和分享/应用 → 将此网站安装为应用。

## 重要
- PWA 安装要求 HTTPS（GitHub Pages 默认提供 HTTPS）。
- GitHub Pages 是静态托管，不负责同步数据。
- 不要把此版本误认为云同步版；本版本明确采用本地保存。
