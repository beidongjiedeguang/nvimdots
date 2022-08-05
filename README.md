安装 neovim:
```
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:neovim-ppa/stable
sudo apt-get update
sudo apt-get install neovim

#pip install neovim
```

终端字体需要使用Nerd Font或者其他有icon字体补丁的font：
https://www.nerdfonts.com/

此外还需要安装ripgrep和fd来配合插件的快速搜索：
```
sudo apt install ripgrep fd-find

```

配置文件:
```
git clone --depth=1 https://github.com/beidongjiedeguang/nvimdots.git ~/.config/nvim/
# git clone --depth=1 git@github.com:beidongjiedeguang/nvimdots.git ~/.config/vim/

```
首次打开nvim, 如果插件clone失败， 使用下面
```
nvim +PackerSync 
```
需要记住的一点是使用`PackerSync`命令才能让你对插件相关的config的修改生效（对config.lua和plugins.lua文件的修改，修改其他文件不需要）

切换到coc配置（如果想要的话）
```
cd ~/.config/nvim
# git switch coc

# 一些插件clone失败后，可以退出重新进入，并使用命令

