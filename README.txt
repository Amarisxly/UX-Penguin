企鹅破题板 · PWA

文件
  index.html            应用本体（已内置 15 块板子和你写过的思考）
  manifest.webmanifest  应用名称、图标、全屏显示设置
  sw.js                 离线缓存
  icons/                像素企鹅图标

怎么上线（任选一种，必须是 https 网址，PWA 才能安装）
  1. Netlify Drop：打开 app.netlify.com/drop，把整个 penguin-pwa 文件夹拖进去，几秒后得到网址。
  2. GitHub Pages：新建仓库，上传这些文件，在 Settings → Pages 里开启。
  3. Vercel / Cloudflare Pages：同样直接上传文件夹即可。
  注意：直接双击 index.html 也能打开，但不能安装、也不能离线。

怎么安装到手机
  iPhone：用 Safari 打开网址 → 分享 → 添加到主屏幕。
  Android：用 Chrome 打开网址 → 菜单 → 安装应用 / 添加到主屏幕。
  电脑：Chrome 或 Edge 地址栏右侧的安装图标。

数据保存在哪里
  这个版本把板子保存在当前设备的浏览器里，离线也能新增、修改、写思考。
  换设备或清理浏览器数据前，请先点“导出备份”，在新设备上点“导入”即可恢复。
  它和 claude.ai 上的在线版是两份独立的数据，不会自动同步。

更新应用后
  修改文件后，把 sw.js 第 2 行的 VERSION 改成新名字（如 poti-v2），用户下次打开就会拿到新版本。
