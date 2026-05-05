# Clash Verge for Arm

Linux `arm64` 平台可用的 Clash Verge Rev Debian 安装包。

本仓库当前提供 `Clash Verge Rev 2.4.7` 的 `arm64` 架构 `.deb` 包，适合在支持 Debian 包管理的 ARM64 Linux 桌面环境中安装使用，例如 Debian、Ubuntu 及其衍生发行版。

## 文件信息

| 项目 | 内容 |
| --- | --- |
| 文件名 | `Clash.Verge_2.4.7_arm64.deb` |
| 包名 | `clash-verge` |
| 版本 | `2.4.7` |
| 架构 | `arm64` |
| 大小 | 约 `51 MB` |
| SHA256 | `35f321a498f762175316b231d2fad3a90678016ad19157779758b5420d743a8f` |

## 下载

可以直接在 GitHub 页面点击 `Clash.Verge_2.4.7_arm64.deb` 下载，也可以使用命令行下载：

```bash
wget https://github.com/CQULzz/Clash-Verge-for-Arm/raw/main/Clash.Verge_2.4.7_arm64.deb
```

## 校验

安装前建议校验文件完整性：

```bash
echo "35f321a498f762175316b231d2fad3a90678016ad19157779758b5420d743a8f  Clash.Verge_2.4.7_arm64.deb" | sha256sum -c -
```

如果输出包含 `OK`，说明文件校验通过。

## 安装

推荐使用 `apt` 安装本地 `.deb` 文件，这样可以自动处理依赖：

```bash
sudo apt update
sudo apt install ./Clash.Verge_2.4.7_arm64.deb
```

该包声明的主要依赖包括：

- `openssl`
- `libayatana-appindicator3-1`
- `libwebkit2gtk-4.1-0`
- `libgtk-3-0`

如果安装时提示依赖缺失，可以先修复依赖后再尝试安装：

```bash
sudo apt --fix-broken install
sudo apt install ./Clash.Verge_2.4.7_arm64.deb
```

## 启动

安装完成后，可以从桌面应用菜单中启动 `Clash Verge`，也可以在终端运行：

```bash
clash-verge
```

## 卸载

```bash
sudo apt remove clash-verge
```

如需同时清理配置文件，可使用：

```bash
sudo apt purge clash-verge
```

## 说明

- 本仓库仅提供 `arm64` 架构的 Debian 安装包。
- 如果你的系统是 `amd64` / `x86_64`，请使用对应架构的安装包。
- 软件功能、内核与界面以安装包实际内容为准。
