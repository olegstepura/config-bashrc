# config-bashrc
My personal system-level bashrc config. Used on ArchLinux primarily, but is easy to use on any linux distro.

To install this I do::
```bash
cd /etc
wget https://github.com/olegstepura/config-bashrc/blob/master/bash.bashrc.local.sh
vim bash.bashrc
```
And add this to the very beginning of the file (actually after first comments in a file to allow syntax discovery by vim):
```
. /etc/bash.bashrc.local.sh && return
```
