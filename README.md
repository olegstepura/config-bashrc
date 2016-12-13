# config-bashrc
My personal system-level bashrc config. Used on ArchLinux primarily, but is easy to use on any linux distro.

To install this I do:
```bash
curl https://raw.githubusercontent.com/olegstepura/config-bashrc/master/bash.bashrc.local.sh -o /etc/bash.bashrc.local.sh
sed -i -e '4i. /etc/bash.bashrc.local.sh && return\' /etc/bash.bashrc
cat /etc/bash.bashrc
```
Second command adds usage of the separate bashrc script in the main system bashrc (to the very beginning of the file, though after first comments in a file to allow syntax discovery by vim).
Cat was inserted to print result so that you can make sure everything is ok.

Or you can download [this file manually](https://github.com/olegstepura/config-bashrc/blob/master/bash.bashrc.local.sh) and edit `/etc/bash.bahsrc` by hand to add this as the first command:
```bash
. /etc/bash.bashrc.local.sh && return
```

Due to security risks this is not recommended to do so, but if you are lazy and have to type commands from first snippet by hand, you can use this (it will download the snippet from above and run in your shell):
```bash
bash <(curl -Ls https://goo.gl/sqo51K)
```
