## spacecode

### 概述

本文档记录个人对于vs code的使用心得

### 使用

- 下载并安装vs code
- 安装插件 VSpaceCode https://github.com/VSpaceCode/VSpaceCode
- 安装之后，这个插件其实是需要修改 setting.json 和 keybinding.json 不过安装之后没有直接修改
- 可以在 Help -> Show All Commands 分别执行 VSpaceCode: Configure Default Settting 和 VSpaceCode: Configure Default Keybinding
- 执行完成之后，就可以看到setting.json和keybinding.json都已经修改并加入配置了
- 接下来其实是个人进一步的一些配置了，因为vspacecode其实应该是在vscodevim的前提下，个人的一些配置在目录下的 settting.json和keybinding.json
- 个人累计安装的一些插件
    - vspacecode
    - center editor window
    - chinese 简体中文
    - go
    - json

### 常见问题

- 发现长按 jk 之类的没有用了，需要一下一下的按
    - https://github.com/VSCodeVim/Vim#mac
    - 执行以下内容
        ```
        $ defaults write com.microsoft.VSCode ApplePressAndHoldEnabled -bool false              # For VS Code
        $ defaults write com.microsoft.VSCodeInsiders ApplePressAndHoldEnabled -bool false      # For VS Code Insider
        $ defaults write com.visualstudio.code.oss ApplePressAndHoldEnabled -bool false         # For VS Codium
        $ defaults write com.microsoft.VSCodeExploration ApplePressAndHoldEnabled -bool false   # For VS Codium Exploration users
        $ defaults delete -g ApplePressAndHoldEnabled                                           # If necessary, reset global default
        ```