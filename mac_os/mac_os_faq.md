# Mac OS FAQ

- [Turn off the rootless in OS X El Capitan 10.11](https://www.quora.com/How-do-I-turn-off-the-rootless-in-OS-X-El-Capitan-10-11)
- 强制使用 32 位：
```
    defaults write com.apple.versioner.python Prefer-32-Bit -bool yes
```
- 去掉强制使用 32 位：
```
    defaults write com.apple.versioner.python Prefer-32-Bit -bool no
```

- 苹果 Mac OS X 显示隐藏文件的方法

    - 早期的OS X（10.6~10.8）系统可以使用如下两条命令来开始或者关闭系统隐藏文件的显示：
    ```
    defaults write com.apple.Finder AppleShowAllFiles Yes && killall Finder //显示隐藏文件
    defaults write com.apple.Finder AppleShowAllFiles No && killall Finder //不显示隐藏文件
    ```
    - 当升级到OS X 10.9 Mavericks版本之后，这两条命令需要做一些修改，变成了如下命令：
    ```
    defaults write com.apple.finder AppleShowAllFiles Yes && killall Finder //显示隐藏文件
    defaults write com.apple.finder AppleShowAllFiles No && killall Finder //不显示隐藏文件
    ```