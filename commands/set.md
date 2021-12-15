# set
## 帮助信息
### 描述

设置或取消设置 Shell 选项和位置参数的值。
更改外壳属性和位置参数的值，或显示外壳变量的名称和值。

### 选项

| Option | Effect                                                                                                                                       |
|--------|----------------------------------------------------------------------------------------------------------------------------------------------|
| `-a`   | 标记为导出而修改或创建的变量                                                                                                                 |
| `-b`   | 立即通知工作终止                                                                                                                             |
| `-e`   | 如果命令以非零状态退出，则立即退出                                                                                                           |
| `-f`   | 禁用文件名生成（globbing）                                                                                                                   |
| `-h`   | 查找命令时，请记住命令的位置                                                                                                                 |
| `-k`   | 所有赋值参数都放置在命令的环境中，而不仅仅是命令名称之前的参数                                                                               |
| `-m`   | 启用作业控制                                                                                                                                 |
| `-n`   | 阅读命令，但不要执行它们                                                                                                                     |
| `-o`   | 设置 option-name 对应的变量                                                                                                                  |
| `-p`   | 每当真实有效的用户 ID 不匹配时，打开。禁用 $ENV 文件的处理和 shell 函<br>数的导入。关闭此选项会导致有效的 uid 和 gid 设置为真正的 uid 和 gid |
| `-t`   | 阅读和执行一个命令后退出                                                                                                                     |
| `-u`   | 将未设置的变量视为替换时的错误                                                                                                               |
| `-v`   | 读取时打印 shell 输入行                                                                                                                      |
| `-x`   | 执行命令及其参数时打印它们                                                                                                                   |
| `-B`   | shell 将执行大括号扩展                                                                                                                       |
| `-C`   | 如果设置了，则不允许通过重定向输出覆盖现有的常规文件                                                                                         |
| `-E`   | 如果设置，ERR陷阱由shell函数继承                                                                                                             |
| `-H`   | 启用 `!` 风格历史替换。当 shell 交互时，默认情况下此标志处于打开状态                                                                         |
| `-P`   | 如果设置了，在执行更改当前目录的cd等命令时，不要解析符号链接                                                                                 |
| `-T`   | 如果设置，DEBUG 和 RETURN 陷阱由 shell 函数继承                                                                                              |
| `--`   | 将任何剩余参数分配给位置参数。如果没有剩余的参数，位置参数将取消设置                                                                         |
| `-`    | 将任何剩余的参数分配给位置参数。 `-x` 和 `-v` 选项已关闭                                                                                     |

| option-name            | Effect                                                                                     |
|------------------------|--------------------------------------------------------------------------------------------|
| `allexport`            | 与 `-a` 相同                                                                               |
| `braceexpand`          | 与 `-B` 相同                                                                               |
| `emacs`                | 使用 emacs 风格的行编辑界面                                                                |
| `errexit`              | 与 `-e` 相同                                                                               |
| `errtrace`             | 与 `-E` 相同                                                                               |
| `functrace`            | 与 `-T` 相同                                                                               |
| `hashall`              | 与 `-h` 相同                                                                               |
| `histexpand`           | 与 `-H` 相同                                                                               |
| `history`              | 启用命令历史                                                                               |
| `ignoreeof`            | shell 不会在读取 EOF 时退出                                                                |
| `interactive-comments` | 允许注释出现在交互式命令中                                                                 |
| `keyword`              | 与 `-k` 相同                                                                               |
| `monitor`              | 与 `-m` 相同                                                                               |
| `noclobber`            | 与 `-C` 相同                                                                               |
| `noexec`               | 与 `-n` 相同                                                                               |
| `noglob`               | 与 `-f` 相同                                                                               |
| `nolog`                | 当前被接受但被忽略了                                                                       |
| `notify`               | 与 `-b` 相同                                                                               |
| `nounset`              | 与 `-u` 相同                                                                               |
| `onecmd`               | 与 `-t` 相同                                                                               |
| `physical`             | 与 `-P` 相同                                                                               |
| `pipefail`             | 管道的返回值是最后一个以非零状态退出的命令的状态，<br>如果没有以非零状态退出的命令，则为零 |
| `posix`                | 更改默认操作与Posix标准不同的bash行为，以匹配标准                                          |
| `privileged`           | 与 `-p` 相同                                                                               |
| `verbose`              | 与 `-v` 相同                                                                               |
| `vi`                   | 使用 vi 风格的行编辑界面                                                                   |
| `xtrace`               | 与 `-x` 相同                                                                               |

## set --help

```shell
set: set [-abefhkmnptuvxBCHP] [-o option-name] [--] [arg ...]
    Set or unset values of shell options and positional parameters.

    Change the value of shell attributes and positional parameters, or
    display the names and values of shell variables.

    Options:
      -a  Mark variables which are modified or created for export.
      -b  Notify of job termination immediately.
      -e  Exit immediately if a command exits with a non-zero status.
      -f  Disable file name generation (globbing).
      -h  Remember the location of commands as they are looked up.
      -k  All assignment arguments are placed in the environment for a
          command, not just those that precede the command name.
      -m  Job control is enabled.
      -n  Read commands but do not execute them.
      -o option-name
          Set the variable corresponding to option-name:
              allexport    same as -a
              braceexpand  same as -B
              emacs        use an emacs-style line editing interface
              errexit      same as -e
              errtrace     same as -E
              functrace    same as -T
              hashall      same as -h
              histexpand   same as -H
              history      enable command history
              ignoreeof    the shell will not exit upon reading EOF
              interactive-comments
                           allow comments to appear in interactive commands
              keyword      same as -k
              monitor      same as -m
              noclobber    same as -C
              noexec       same as -n
              noglob       same as -f
              nolog        currently accepted but ignored
              notify       same as -b
              nounset      same as -u
              onecmd       same as -t
              physical     same as -P
              pipefail     the return value of a pipeline is the status of
                           the last command to exit with a non-zero status,
                           or zero if no command exited with a non-zero status
              posix        change the behavior of bash where the default
                           operation differs from the Posix standard to
                           match the standard
              privileged   same as -p
              verbose      same as -v
              vi           use a vi-style line editing interface
              xtrace       same as -x
      -p  Turned on whenever the real and effective user ids do not match.
          Disables processing of the $ENV file and importing of shell
          functions.  Turning this option off causes the effective uid and
          gid to be set to the real uid and gid.
      -t  Exit after reading and executing one command.
      -u  Treat unset variables as an error when substituting.
      -v  Print shell input lines as they are read.
      -x  Print commands and their arguments as they are executed.
      -B  the shell will perform brace expansion
      -C  If set, disallow existing regular files to be overwritten
          by redirection of output.
      -E  If set, the ERR trap is inherited by shell functions.
      -H  Enable ! style history substitution.  This flag is on
          by default when the shell is interactive.
      -P  If set, do not resolve symbolic links when executing commands
          such as cd which change the current directory.
      -T  If set, the DEBUG and RETURN traps are inherited by shell functions.
      --  Assign any remaining arguments to the positional parameters.
          If there are no remaining arguments, the positional parameters
          are unset.
      -   Assign any remaining arguments to the positional parameters.
          The -x and -v options are turned off.

    Using + rather than - causes these flags to be turned off.  The
    flags can also be used upon invocation of the shell.  The current
    set of flags may be found in $-.  The remaining n ARGs are positional
    parameters and are assigned, in order, to $1, $2, .. $n.  If no
    ARGs are given, all shell variables are printed.

    Exit Status:
    Returns success unless an invalid option is given.
```
