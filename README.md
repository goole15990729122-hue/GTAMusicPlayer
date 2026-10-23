# GTA Music Player Android 项目

根据提供的 GTA 风格播放器模板制作的原生 Android 项目。

## 功能
- GTA 风格深色界面与荧光黄点缀
- 欢迎页、首页、本地歌曲列表、搜索、我的页面、播放页
- 请求系统音频权限并扫描本地音乐媒体库
- 播放、暂停、上一首、下一首、搜索歌曲/艺术家/专辑
- GitHub Actions 自动构建 APK

## 如何得到 APK
1. 在 GitHub 新建一个空仓库。
2. 解压此 ZIP，将里面所有文件（包括隐藏的 `.github` 文件夹）上传到仓库根目录并提交到 `main` 分支。
3. 打开仓库的 **Actions** 标签，选择 **Build Android APK**，点击 **Run workflow**。如果按钮没出现，先提交文件后刷新。
4. 构建成功后打开该次运行页面，在 **Artifacts** 下载 `GTA-Music-Player-APK`。
5. 解压 Artifact，得到 `app-debug.apk`，传到 Android 手机安装。

Windows 查看隐藏文件：文件资源管理器 → 查看 → 显示 → 隐藏的项目。

## 注意
这是调试签名 APK 的构建工程，并非 Play 商店发布签名包。本执行环境没有 Android SDK/Gradle，不能直接在这里编译 APK；使用 GitHub Actions 云端构建。部分手机可能需要允许安装未知来源应用。
