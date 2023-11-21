# pikvm

### Boot error on systemD PIROOT disk label query

As discussed in : https://github.com/pikvm/pikvm/issues/982
A non-reactive system drive will cause the arch distribution to boot into the emergency shell.

The workaround to this issue is to edit the pikvm image's config.txt file to replace `ROOT=LABEL=PIROOT` to `ROOT=/dev/disk/by-label/PIROOT`



