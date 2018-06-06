# MMC utils for Android


## mmc-utils - Configure MMC storage devices from userspace.

    mmc [<command> [<args>]] [--help]
    mmc [<command>] --help

mmc-utils is a tool for configuring MMC storage devices from userspace.

## COMMANDS AND OPTIONS

Shows the abbreviated help menu in the terminal:
      
      help | --help | -h | (no arguments)
      
Print extcsd data from device:
      
      extcsd read <device>
      


Example to get the Life time or EOL status,
      
      mmc extcsd read /dev/mmcblk1 | grep -i life
      mmc extcsd read /dev/mmcblk1 | grep -i eol
      