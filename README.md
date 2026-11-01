# PCL Hanaka（第三方修改）

> 本仓库是**第三方基于 Plain Craft Launcher 独立进行二次创作**的产物，与原作者龙腾猫跃及 PCL 官方无关。
>
> - 上游：<https://github.com/Meloong-Git/PCL>，本次基于 `main` 分支提交 `93ede5d`（版本 2.99.0.1）
> - 许可：继续沿用上游 [LICENCE](LICENCE)（《PCL 分发有限许可》），未作改动

## 相对上游的修改

1. **名称**：窗口标题、关于页、程序集信息统一为 `PCL Hanaka（第三方修改）`。
2. **关于页**：保留「龙腾猫跃」署名与赞助链接在首位，补充「第三方独立创作，与龙腾猫跃无关」说明，新增上游源码与本仓库源码入口。
3. **构建可复现化**：主工程 `Plain Craft Launcher 2.vbproj` 改用 `PCLCS\bin` 预编译产物代替 ProjectReference，显式指定源文件编码 UTF-8 与 `netstandard` 门面引用，便于在没有 Visual Studio 的环境里构建（见 `../build-pcl-hanaka.ps1`）。
4. **配色**：改为「靛蓝」方案（`Modules\ModSecret.vb` 里的 `ForkColorHue/Sat/LightAdjust/TopbarDelta` 四个常量控制整套配色，当前 Hue=224、Sat=78、明度 -2）。仍属蓝色系，符合许可第 5 条。
5. **未改动**：下载 / 启动 / 联机等全部功能逻辑；未新增任何赞助解锁类功能；`McLaunchPrecheck` 的正版购买劝导逻辑保持原样。

## 上游说明（原文摘录）

包含 PCL 的大部分源代码，包括 UI 库、动画模块、下载模块、Minecraft 启动模块等。

代码并不是实时更新的，它会在每次 PCL 发布更新时同步一次。

## 相关资源

- 上游项目：<https://github.com/Meloong-Git/PCL>
- 上游作者赞助：<https://meloong.com/afd/a/LTCat>
