#亚行

[[需要按住移动]]

更多信息请查看

Android开发者

。

您可能需要关闭 系统设置 - “安全” - “Secure app spawning”。

[来源](https://github.com/RikkaApps/websites/pull/79#issue-1751837442)

:::

### 通过 root 启动

如果您的设备已经 root，直接启动即可。

### 通过无线调试启动

通过无线调试启动适用于 Android 11 或以上版本。这种启动方式无需连接电脑。由于系统限制，每次重新启动后都需要再次进行启动步骤。

#### 启用无线调试

1. 在网络上搜索如何为您的机型启用“开发者选项”
2. 启用“开发者选项”和“USB 调试”<溴><溴><百万毫克:src="$withBase('/images/enable_dev_options.png')" 风格="max-width:320小卖部;宽度:100%">
3.马克
4.打开文件夹，右键选择
   
Windows 10:在此处打开 PowerShell

1.在 Shizuku you you you“you”“you”“com”：src="$withBase（'/images/start_paring_from_Shizuku.png'）""max="max-width:320；100％"
2. [需要按住移动](）)
Windows 7:在此处打开命令行窗口[需要按住移动]）
Mac或 Linux:you mayota终端（）

输入

亚行

如果可以看到一长串内容而不是提示找不到亚行

：提示提示

请不要关闭该窗口，后面提到的“终端”都是指此窗口（如果关闭请重新进行第 2 步）。

####如果使用 PowerShell`亚行`用户手册

Orranic碳总量（toc）`##启动 Shizuku`静久支持通过以下三种方式启动

：提示如果您正在使用 GrapheneOS[您可能需要关闭 mayoto-“mayoto”-“安全应用程序产卵”](https://developer.android.google.cn/studio/command-line/adb)来源

####通过 root`如果您的设备已经根，站在前面`

1.通过无线调试启动

   * [通过无线调试启动适用于安卓11你要把它放在你的面前吗](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)
   * [启用无线调试](https://dl.google.com/android/repository/platform-tools-latest-linux.zip)
   * [在网络上搜索如何为您的机型启用“开发者选项”](https://dl.google.com/android/repository/platform-tools-latest-darwin.zip)

2.启用“you you you mayoto”“USB you you”“you you”“you”<><><src:src="$withBase（'/images/enable_dev_options.png'）"="max-width:320；：100％">

   *进入“you you mayou mayou”“you you”“you you you”“src="$withBase（'/images/enter_wireless_debugging.png'）”="max-width:320；：100％">**启用“you you mayou”“you you you”“you you”“you you you”“src：src="$withBase（'/images/enable_wireless_debugging.png'）"="max-width:320；：100％">**####配对（仅需一次）
   * Windows 7：在此处打开命令行窗口（**需要按住 Shift 才会显示该选项**）
   *该启动方式适用于未 root在我的面前，我站在了前面

3.什么是`亚行`？

Android调试桥
1.亚行
2.）是一个通用命令行工具，在我的前面，我的前面，我的前面，我的前面`更多信息请查看`Android开发者`./adb`。
:::

####安装`亚行`

下载由谷歌你喜欢什么`窗`Linux

1. 打开系统设置，进入关于
2. 连续数次点击 "Build number" 后看到类似 "You are a developer" 的提示
3. 此时你应该可以在设置中找到“开发者选项”，进入后开启“USB 调试”
4. 连接设备到电脑，在终端中输入 `adb devices`
5. 此时设备上会出现“是否允许调试”的对话框，勾选“总是允许”后确认
6. 再次在终端中输入 `adb devices`，如无问题将会看到类似如下内容
   ```
   List of devices attached
   XXX      device
   ```

::: tip
不同设备开启“开发者选项”的步骤可能有所不同，请自己搜索。
:::

#### 启动 Shizuku

复制指令并粘贴到终端中，如无问题你将会在 Shizuku 中看到已启动成功。

::: details 适用于 Shizuku v11.2.0+ 的指令 

```
adb shell sh /sdcard/Android/data/moe.shizuku.privileged.api/start.sh
```
:::

## 常见问题

许多厂商对 Android 系统进行了修改，这会造成 Shizuku 无法正常工作。

### 通过无线调试启动：一直显示“正在搜索配对服务”

请允许 Shizuku 在后台运行。

搜索配对服务需要访问本地网络，许多厂商在应用不可见后立刻禁止应用访问网络。您可以在网络上搜索如何在您的设备上允许应用在后台运行。

### 通过无线调试启动：点击“输入配对码”后立刻提示失败

#### MIUI（小米、POCO）

在系统设置的“通知管理”-“通知显示设置”将通知样式切换为“原生样式”。

### 通过无线调试启动/通过连接电脑启动：adb 权限受限

#### MIUI（小米、POCO）

在“开发者选项”中开启“USB 调试（安全设置）”。**注意，这和“USB 调试”是两个分开的选项。**

#### ColorOS（OPPO & OnePlus）

在“开发者选项”中关闭“权限监控”。

#### Flyme（魅族）

在“开发者选项”中关闭“Flyme 支付保护”。

### 通过无线调试启动/通过连接电脑启动：Shizuku 随机停止

#### 所有设备

- 保证 Shizuku 可以在后台运行。
- 不要关闭“USB 调试”及“开发者选项”。
- 在“开发者选项”中将 USB 使用模式改为“仅充电”。
  
  在 Android 8 上的选项是“选择 USB 配置”-“仅充电”。
  
  在 Android 9 及以上版本上选项是“默认 USB 配置”-“不进行数据传输”。

- （Android 11+）启用“停用 adb 授权超时功能”选项

#### EMUI (华为) 

在“开发者选项”中开启「“仅充电”模式下允许 ADB 调试选项」。

#### MIUI（小米、POCO）

不要使用“手机管家”的扫描功能，因为它会禁用开发者选项。

#### Sony

不要点击连接 USB 后弹出的对话框，因为这会导致 USB 使用模式发生变化。

### 通过 root 启动：无法开机启动

请允许 Shizuku 在后台运行。
