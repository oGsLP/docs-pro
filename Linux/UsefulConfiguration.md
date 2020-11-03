# Useful Configurations

## Permission 权限

- 设置用户的 root 权限， sudo 免密

  - `sudo visudo`
  - `在 root ALL = (ALL) ALL`行下添加 `username ALL = (ALL) NOPASSWD:ALL`

## alias

- 配置 alias

  - 在用户目录下添加`.bash_alias`文件
  - 在`.bashrc`中加入

    ```shell
    if [ -f ~/.bash_alias ]; then
      . ~/.bash_alias
    fi
    ```

  - 在.bash_alias 中添加自定义的 alias

- 个人alias推荐

	- 暴力删除alias
		- `alias rmrf='sudo rm -rf'