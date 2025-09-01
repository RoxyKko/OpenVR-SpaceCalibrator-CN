<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/hyblocker/OpenVR-SpaceCalibrator/blob/develop/.github/logo_light.png?raw=true">
  <source media="(prefers-color-scheme: light)" srcset="https://github.com/hyblocker/OpenVR-SpaceCalibrator/blob/develop/.github/logo_dark.png?raw=true">
  <img alt="Space Calibrator" src="https://github.com/hyblocker/OpenVR-SpaceCalibrator/blob/develop/.github/logo.png?raw=true">
</picture>

此程序旨在帮助您在 SteamVR 中同步多个游戏空间。Space Calibrator (spacecal) 的这个分支也支持[连续校准](#continuous-calibration)。

连续校准是一种追踪模式，它使用头戴设备上的追踪器自动将游戏空间对齐。

## 安装教程

### Steam

> [!NOTE]  
> **Space Calibrator 也可在 Steam 上使用。**

你可以在Steam的这里找到 [Space Calibrator on Steam here](https://s.team/a/3368750).

### 从 GitHub 获取

要安装 Space Calibrator，请从下载页面获取最新的安装程序并安装。请确保您已安装：

- 已安装 [Visual C++ Redistributable](https://aka.ms/vs/17/release/vc_redist.x64.exe)。
- 安装 SteamVR 并在连接 VR 耳机的情况下至少运行一次。
- 运行安装程序之前，SteamVR 尚未运行。如果 SteamVR 正在运行，安装程序将无法正确安装 Space Calibrator。

## 定期校准(Calibration)

如果您不想使用连续校准，则必须使用定期校准。这意味着您需要不时地将耳机的游戏空间与追踪器的游戏空间同步。

校准方法：

1. 复制头戴设备（HMD）游戏区域的安全边界/防护系统设置

   > **此操作仅需执行一次。** 连接您的 VR 头戴设备并启动 SteamVR。然后找到 Space Calibrator 的窗口（它可能会被最小化），点击 "Copy Chaperone" (复制安全边界) 按钮。

2. 打开 SteamVR 控制面板 (dashboard)。在底部，点击 Space Calibrator 图标。

3. 在 Space Calibrator 的叠加界面 (overlay) 中，顶部会显示两个列表。在左侧的 `Reference Space` (参考空间) 栏中，选择您要用来进行校准的控制器（例如 Quest 控制器、Pico 控制器）。在右侧的 `Target Space` (目标空间) 栏中，选择您的 SteamVR 追踪器（例如 Vive Ultimate Tracker, Vive Tracker 3.0, Vive Ultimate Tracker）。您可以使用 "Identify" (识别) 按钮让控制器闪烁和追踪器的 LED 灯闪烁，以确认选择是否正确。

4. 点击 "Start calibration" (开始校准) 按钮，即可开始校准。

## 连续校准 (Continuous Calibration)

> [!重要]
> ****此模式需要将一个tracker追踪器附着在您的头戴设备上。****

要启用连续校准模式，首先在左侧栏中选择您的头戴设备，然后在右侧栏中选择附着在头戴设备上的追踪器。完成此操作后，点击 `Start Calibration` (开始校准)，然后点击 `Cancel` (取消)。接着点击 `Continuous Calibration` (连续校准) 来启用连续校准模式。

1. 启动您想要使用的 VR 头戴设备对应的 SteamVR。
2. **仅** 开启附着在 VR 头戴设备上的那个追踪器。
3. 选择该 VR 头戴设备和追踪器并进行校准。
4. 开启您的其他设备。
5. 您应该会看到，在您于游戏区域内移动一会儿完成初始校准后，这些设备会与您（的动作）对齐。

## 帮助

如果您在此程序设置过程中需要帮助，请查阅 [项目 Wiki](https://github.com/pushrax/OpenVR-SpaceCalibrator/wiki) 或加入 [Discord 服务器](https://discord.gg/ja3WgNjC3z)。

## 版本差别与致谢

> 转自reddit：[您应该使用哪个版本的 OpenVR Space Calibrator？](https://www.reddit.com/r/MixedVR/comments/19ay1bp/which_version_of_openvr_space_calibrator_should/)
>
> 如同其在开头所叙述的，分享这个信息是为了让其他人了解不同的分支和版本（截至 2025 年 8 月）并记录和感谢这些伟大无私的开源开发者

#### pushRax

> OpenVR-SpaceCalibrator最初的开发者为 **pushRax** 

OpenVR-SpaceCalibrator 1.4 版本由 **pushRax** 开发，最新更新时间为**2022 年 3 月 31 日**

https://github.com/pushrax/OpenVR-SpaceCalibrator

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/pin/?username=pushRax&repo=OpenVR-SpaceCalibrator&theme=radical" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api/pin/?username=pushRax&repo=OpenVR-SpaceCalibrator" />
    <img alt="Repo Card" src="https://github-readme-stats.vercel.app/api/pin/?username=pushRax&repo=OpenVR-SpaceCalibrator" />
  </picture>

从那时起，一个经常被提及的分支被创造出来，它通过使用连接到头显的追踪器不断重新校准， ***显著减少了追踪器漂移。这真是太棒了。***

#### bdunderscore

> 后来由**bdunderscore** 接手，fork并添加了新功能

**添加连续堆叠的bdunderscore** fork 的最后一个版本是 v1.4-bd_-r2 - 最后更新于 2022 年 9 月 26 日

https://github.com/bdunderscore/OpenVR-SpaceCalibrator

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/pin/?username=bdunderscore&repo=OpenVR-SpaceCalibrator&theme=radical" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api/pin/?username=bdunderscore&repo=OpenVR-SpaceCalibrator" />
    <img alt="Repo Card" src="https://github-readme-stats.vercel.app/api/pin/?username=bdunderscore&repo=OpenVR-SpaceCalibrator" />
  </picture>

很遗憾，bdunderscore 的分支已**不再维护**。2022 年 9 月 15 日，bdunderscore 发帖称： *“嗨！此分支目前无人维护，因为我没时间维护（而且目前不使用 Quest 无线）。请随意继续创建分支，并根据自己的情况进行修复。”*

#### ArcticFox8515

> **bdunderscore**的分支版本对于三个tracker+头显的一个辅助校准tracker表现已经良好，但对于更多的tracker，如6个tracker+头显的一个辅助校准tracker，会由于追踪延迟出现些许不稳定的现象。
> 	后来，**ArcticFox8515**接手了这项工作，并于 2023 年 5 月 30 日从 bdunderscore 版本中分叉出来；当前版本为v1.4-bd_+af-r7，最后更新于 2024 年 10 月 23 日

**ArcticFox8515**的版本彻底解决了多tracker下跟踪延迟的问题。

https://github.com/ArcticFox8515/OpenVR-SpaceCalibrator

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/pin/?username=ArcticFox8515&repo=OpenVR-SpaceCalibrator&theme=radical" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api/pin/?username=ArcticFox8515&repo=OpenVR-SpaceCalibrator" />
    <img alt="Repo Card" src="https://github-readme-stats.vercel.app/api/pin/?username=ArcticFox8515&repo=OpenVR-SpaceCalibrator" />
  </picture>

#### hyblocker

从那时起，就有了更新的版本。**hyblocker**从**ArcticFox8515**版本fork，并于 2023 年 12 月 6 日发布了 v1.4-bd_+af-r7

https://github.com/hyblocker/OpenVR-SpaceCalibrator

<picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/pin/?username=hyblocker&repo=OpenVR-SpaceCalibrator&theme=radical" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api/pin/?username=hyblocker&repo=OpenVR-SpaceCalibrator" />
    <img alt="Repo Card" src="https://github-readme-stats.vercel.app/api/pin/?username=hyblocker&repo=OpenVR-SpaceCalibrator" />
  </picture>



目前**hyblocker**发布的最新版本为2024年12月5日发布的1.5.1版本，本汉化版本即是基于**hyblocker**发布的1.5.1版本进行文本汉化

> 截止至进行汉化工作的2025年9月1日，从**hyblocker**的项目git记录中发现**hyblocker**在29.Aug.2025仍有更新，相信未来的不久**hyblocker**就会发布一个新的版本



## 赞助我一包小零食

<p align="center">
  <img src="./pic/weixin.jpg" alt="微信" width="30%" />
  <img src="./pic/zhifubao.jpg" alt="支付宝" width="30%" />
</p>