# macOS

## Install Oh-my-zsh

[oh-my-zsh国内镜像安装和更新方法](https://www.jianshu.com/p/6b47198fd430)

## Install Homebrew

[清华大学开源软件镜像站-Homebrew / Linuxbrew 镜像使用帮助](https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/)

Update `.zshrc`.

```
export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles
```

## Install Desktop Application

```
brew install visual-studio-code
brew install hammerspoon
brew install iterm2
brew install alfred
```

- Docker
- IntelliJ idea

## Install CLI application

```
brew install ack diff-so-fancy fd fzf go gradle htop jenv jq maven mosh ncdu nvm openjdk python ruby sbt tig tldr tmux tree wget
```

## Update Hammerspoon script

Make window manager.

```
md ~/.hammerspoon
```

Copy [init.lua](./init.lua) to `~/.hammerspoon`.

## Install JDK

Download sdks from [adoptopenjdk](https://adoptopenjdk.net/).

```shell
md ~/Library/Java/JavaVirtualMachines
cd ~/Library/Java/JavaVirtualMachines
wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_mac_hotspot_8u292b10.tar.gz # jdk 1.8
wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_mac_hotspot_11.0.11_9.tar.gz # jdk 11
wget https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_mac_hotspot_16.0.1_9.tar.gz # jdk 16
tar xf *.tar.gz
```

```shell
jenv add jdk-xxx
jenv global 11
```
