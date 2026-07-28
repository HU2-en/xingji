# 星寄公网部署包

这个文件夹可以直接上传到 Vercel、Netlify 或 GitHub Pages。部署成功后，你会得到一个公网链接；打开这个链接后，会进入 WorkBuddy 风格的星寄入口，并自动弹出星寄悬浮球工作台。

## 文件说明

```plaintext
index.html          星寄云端入口页
xingji-widget.js   星寄悬浮球工作台组件
404.html           GitHub Pages 兜底入口
.nojekyll          GitHub Pages 静态文件标记
vercel.json        Vercel 配置
netlify.toml       Netlify 配置
package.json       可选项目说明和本地预览命令
README.md          本说明
```

## Vercel 上传方式

1. 打开 Vercel 官网并登录。
2. 新建 Project。
3. 上传本文件夹，或把本文件夹放进 GitHub 仓库后导入。
4. Framework 选择 Other / Static。
5. Build Command 留空。
6. Output Directory 填 `.` 或留空。
7. 部署完成后，Vercel 会给你一个公网链接。

## Netlify 上传方式

1. 打开 Netlify 官网并登录。
2. 进入 Sites。
3. 选择手动上传部署。
4. 直接拖拽这个文件夹。
5. 部署完成后，Netlify 会给你一个公网链接。

## GitHub Pages 上传方式

1. 新建一个 GitHub 仓库，例如 `xingji`。
2. 把本文件夹里的所有文件上传到仓库根目录。
3. 进入仓库 Settings。
4. 打开 Pages。
5. Source 选择 `Deploy from a branch`。
6. Branch 选择 `main`，目录选择 `/root`。
7. 保存后等待几分钟，会得到一个类似 `https://你的用户名.github.io/xingji/` 的链接。

## 数据保存说明

星寄当前使用浏览器本地存储保存数据。只要你使用同一个浏览器访问同一个部署链接，数据会保留并恢复。

如果你换浏览器、换设备，或者在豆包、DeepSeek 的内置浏览器中打开，数据可能不会和原浏览器共享。后续如果要跨设备同步，需要再做账号登录和云端数据库。
