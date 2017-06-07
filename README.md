# wsl-terminal 设置
[wsl-terminal](https://github.com/goreliu/wsl-terminal) settings

## 更换源
* 备份源列表 
``` shell
$ sudo cp /etc/apt/sources.list /etc/apt/sources.list_backup
```

* 更换源，编辑 `/etc/apt/sources.list`，用 `./sources.list` 中的替换(163源)
* 更新
``` shell
$ sudo apt-get update
```

## 终端配色方案
* wsl-terminal->option->Terminal，Type选择`xterm-256color`
* 为终端使用[Solarized](http://www.cnblogs.com/RandyXu/p/3279090.html)配色方案
    - 设置 [solarized theme for GNU ls](https://github.com/seebi/dircolors-solarized), 给 Solarized 增加目录 ls 的颜色方案
    ``` shell
    $ git clone git://github.com/seebi/dircolors-solarized.git
    $ cp ~/dircolors-solarized/dircolors.256dark ~/.dircolors
    $ eval 'dircolors .dircolors'
    ```

    - 编辑 `.bashrc`，添加 `export TERM=xterm-256color`
    - 重新打开 wsl-terminal, 尝试 `ls`, 配色方案应该已经更改
    - wsl-terminal->option->Looks, Theme选择喜欢的主题(base16-oceanicnext.minttyrc就不错)

## Vim
* [vimrc](https://github.com/pkuliubin/vimrc)

## 编程环境

