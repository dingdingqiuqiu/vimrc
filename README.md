### 目录
```
nvim -- nvim配置(~/.config/nvim)
vimrc -- vimrc配置(/etc/vim/vimrc)
```

### 操作
linux系统可以使用`update-alternatives`管理不同版本的编辑器。
通过这个工具，可以轻松切换vim编辑器

首先，将neovim添加到`update-alternatives`系统中
```bash
sudo update-alternatives --install /usr/bin/vim vim /usr/bin/nvim 100
```

`/usr/bin/vim`是`vim`真实路径，`vim`表示vim这个组，`/usr/bin/nvim`是这个组`vim`的一个候选，优先级为100


```bash
sudo update-alternatives --config vim
```

列出所有注册的`vim`的版本，你可以选择程序作为默认`vim`

```bash
vim -v
```

验证`vim`版本

neo:

```bash
sudo update-alternatives --install /usr/bin/vim vim /opt/nvim-linux64/bin/nvim 120
```

### 必需软件
- unzip:解压lsp
- Hack Nerd Fond:nvim-web-devicons文档树所需图标显示 
> 以下是安装命令
```bash
# git 克隆字体库
git clone https://github.com/ryanoasis/nerd-fonts.git --depth 1
# 打开文件夹
cd nerd-fonts
# 安装字体
./install.sh
```

