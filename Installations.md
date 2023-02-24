# checking lxd and lxc installed or not
`which lxc`
`which lxd`
`dpkg -l | grep lxd`

# installation in ubuntu
`sudo apt install lxd`

# checking process
`systemctl start lxd`
`systemctl enable lxd`
`lxc version`

# printing group contents of lxd
`getent group lxd`

# adding normal user to lxd group
`sudo gpasswd -a dinesh lxd`

# to reload group
`newgrp lxd`

# initializing lxd environment
`lxd init`

`lxc help`