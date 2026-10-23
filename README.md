# 吉利星瑞 E01 · Geely Xingrui E01 CarPlay

2021 款**吉利星瑞**车机的 CarPlay 接收端。车机是亿咖通 **E01**（ECARX E01 / FS11），系统 **GKUI 19**，联发科 **MT6735**，**Android 5.1（API 22）**。

源码、问题上报和最新安装包都在 **[DiPlay-Geely-E01](https://github.com/MarioZero99/DiPlay-Geely-E01)**。

👉 **[前往 Releases 列表下载最新安装包与查看更新日志](https://github.com/MarioZero99/DiPlay-Geely-E01/releases)**

没有 Apple 认证，和吉利、亿咖通也没有关系。CarPlay 的名字和图标属于 Apple。

## 这台车机

| | |
|---|---|
| 车型 | 2021 吉利星瑞（Geely Xingrui） |
| 车机 | 亿咖通 E01 / ECARX E01，FS11 |
| 系统 | GKUI 19，Android 5.1（API 22） |
| 芯片 | 联发科 MT6735 |
| 屏幕 | 1920×720 |

## 现在能做什么

- **有线 CarPlay**：USB 数据线插车机数据口。
- **无线 · 车载热点（推荐）**：车机开热点，iPhone 连上后蓝牙配对。
- **无线 · 同一 Wi-Fi**：车机和 iPhone 在同一个 Wi-Fi 里再配对。
- **方向盘**：上一首 / 下一首。那个位置没有播放/暂停，它是车机的飞屏键。
- **三指快捷条**：投屏画面里三指向下滑，可以断开、选导航音频、切日夜、退出。

无线会临时替换车机正在运行的蓝牙进程，**不写 `/system`**，重启车机后原进程回来。不想接受这一点，就用有线。有线不碰蓝牙。

完整说明、截图和风险见 [项目 README](https://github.com/MarioZero99/DiPlay-Geely-E01/blob/main/README.md)。

## 安装

车机要允许安装未知来源的 APK。从别的 DiPlay 换到这一支，签名不同，要先卸载。卸载会清掉分辨率、音频缓冲和保存的 Wi-Fi。以后还用这一支的新版本，可以直接覆盖。

```sh
adb uninstall com.shihab.diplay
adb install -r DiPlay-Legacy-Geely-*.apk
```

没有 ADB 时，把 APK 拷到 U 盘，用车机文件管理器安装。

## English

CarPlay receiver for the **2021 Geely Xingrui** head unit: **ECARX E01**, GKUI 19, MediaTek MT6735, Android 5.1 (API 22).

Source, issues, and releases: **[DiPlay-Geely-E01](https://github.com/MarioZero99/DiPlay-Geely-E01)** · **[Releases](https://github.com/MarioZero99/DiPlay-Geely-E01/releases)**.

Not Apple-certified, and not affiliated with Geely or ECARX. CarPlay is a trademark of Apple Inc.
