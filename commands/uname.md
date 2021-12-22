# uname
## 描述

打印某些系统信息。没有选项，与 `-s` 相同。

## 选项

| Option                      | Effect                                                       |
|-----------------------------|--------------------------------------------------------------|
| `-a`, `--all`               | 按以下顺序打印所有信息，如果未知，请省略 `-p` 和 `-i` 除外： |
| `-s`, `--kernel-name`       | 打印内核名称                                                 |
| `-n`, `--nodename`          | 打印网络节点主机名                                           |
| `-r`, `--kernel-release`    | 打印内核发行版本                                             |
| `-v`, `--kernel-version`    | 打印内核版本                                                 |
| `-m`, `--machine`           | 打印计算机硬件名称                                           |
| `-p`, `--processor`         | 打印处理器类型（非便携式）                                   |
| `-i`, `--hardware-platform` | 打印硬件平台（非便携式）                                     |
| `-o`, `--operating-system`  | 打印操作系统                                                 |
| `--help`                    | 显示此帮助并退出                                             |
| `--version`                 | 输出版本信息并退出                                           |

## uname --help

```shell
Usage: uname [OPTION]...
Print certain system information.  With no OPTION, same as -s.

  -a, --all                print all information, in the following order,
                             except omit -p and -i if unknown:
  -s, --kernel-name        print the kernel name
  -n, --nodename           print the network node hostname
  -r, --kernel-release     print the kernel release
  -v, --kernel-version     print the kernel version
  -m, --machine            print the machine hardware name
  -p, --processor          print the processor type (non-portable)
  -i, --hardware-platform  print the hardware platform (non-portable)
  -o, --operating-system   print the operating system
      --help     display this help and exit
      --version  output version information and exit

GNU coreutils online help: <https://www.gnu.org/software/coreutils/>
Full documentation at: <https://www.gnu.org/software/coreutils/uname>
or available locally via: info '(coreutils) uname invocation'
```
