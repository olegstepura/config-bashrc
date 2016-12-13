# config-bashrc
My personal system-level bashrc config. Used on ArchLinux primarily, but is easy to use on any linux distro.

To install this I do::
```bash
curl https://raw.githubusercontent.com/olegstepura/config-bashrc/master/bash.bashrc.local.sh -o /etc/bash.bashrc.local.sh
sed -i -e '4i. /etc/bash.bashrc.local.sh && return\' /etc/bash.bashrc
cat /etc/bash.bashrc
```
Second command adds usage of the separate bashrc script in the main system bashrc (to the very beginning of the file, though after first comments in a file to allow syntax discovery by vim).
Cat was inserted to print result so that you can make sure everything is ok.

If you have to type command above, use this:
```bash
curl https://goo.gl/x1PFv2 -o /etc/bash.bashrc.local.sh
sed -i -e '4i. /etc/bash.bashrc.local.sh && return\' /etc/bash.bashrc
cat /etc/bash.bashrc
```
