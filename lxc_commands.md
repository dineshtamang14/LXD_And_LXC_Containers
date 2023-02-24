# lxc help command
`lxc help command-name` eg. `lxc help storage`
`lxc storage list`

# listing lxc remote images url
`lxc remote list`

# listing local images
`lxc image list`

# listing all the images
`lxc image list images:` or for specific image `lxc image list images:cent | less`

# to check host kernet
`uname -r`

# to launch a image
`lxc launch ubuntu:16.04 container-name`

# listing a running containers
`lxc list`

# to start/stop a container
`lxc stop container-name` or `lxc start container-name`

# to delete container
`lxc delete container-name`

# to copy a running container
`lxc copy container-name new-container-name`

# to move lxc container
`lxc move container-name different-container-name`

# to get a shell access in lxc container
`lxc exec container-name bash`

# to get a shell access with different user
`lxc exec container-name su - ubuntu`

# to check os release
`lsb_release -dirc`

# to check how many cpu's
`nproc`

# to ping another container 
`ping container-name.lxd`

# to container details
`lxc info container-name | less`

# printing a process tree
`pstree -p 7629`

# to print machine configuration
`lxc config show container-name | less`