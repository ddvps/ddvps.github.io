# Git.BETA.GS

Git.BETA.GS 是一个提供一键重装系统脚本的工具平台，特别适合国内外VPS用户。通过使用该工具，用户可以快速、方便地重新安装操作系统，并支持多种系统镜像和配置选项。下面是该平台的主要功能和相关说明。

## 功能

- 提供 **一键DD脚本**，支持多种操作系统的安装，包括 **Debian**, **Ubuntu**, **CentOS**, **Rocky**, **Windows** 等。
- 支持 **国内和国外镜像源**，并针对国内用户优化了镜像下载，解决了访问速度慢的问题。
- 可以自定义安装过程中的 **SSH端口** 和 **系统密码**，并支持特殊字符的密码。
- 允许用户通过选择不同的系统镜像（如 **41合1镜像**）来重装系统。

## 页面结构

### 标题部分

页面顶部是一个导航栏，展示了以下几个主要链接：
- [首页](https://git.beta.gs/)
- [一键DD脚本[旧版]](https://git.beta.gs/index.php/8.html)
- [关于](https://git.beta.gs/index.php/about.html)

### 主要内容部分

页面的核心部分展示了 "一键DD脚本" 功能，包含以下几个重要部分：

1. **系统介绍**  
   该工具提供一个方便的接口，帮助用户选择和安装各种操作系统，并支持根据用户需要提供不同的配置选项。

2. **更新说明**  
   - 2023年3月13日：新增强制 CN 模式，支持国内主机安装。
   - 2022年7月24日：更新并增加了大量系统镜像，41合1脚本。
   - 2022年7月3日：新增自定义 SSH 端口选项（9-16）。

3. **安装步骤**
   - **Debian/Ubuntu**：使用以下命令安装所需组件：
     ```bash
     apt-get install -y xz-utils openssl gawk file wget screen && screen -S os
     ```
   - **RedHat/CentOS**：
     ```bash
     yum install -y xz openssl gawk file glibc-common wget screen && screen -S os
     ```

4. **下载脚本并执行**
   使用 `wget` 命令下载并执行重装脚本：
   ```bash
   wget --no-check-certificate -O NewReinstall.sh https://raw.githubusercontent.com/fcurrk/reinstall/master/NewReinstall.sh && chmod a+x NewReinstall.sh && bash NewReinstall.sh
   ···
