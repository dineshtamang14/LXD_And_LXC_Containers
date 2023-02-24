# to list all the lxc profiles
`lxc profile list`

# to print details of specific profile
`lxc profile show default`

# copying default profile
`lxc profile copy default custom-profile`

# launching container with profile
`lxc launch ubuntu:16.04 myUbuntu --profile=custom-profile`

# limiting lxc container memory and cpu
# for memory Dynamically
`lxc config set container-name limits.memory 512MB`

# for cpu Dynamically
`lxc config set container-name limits.cpu 1`

# printing configuration details
`lxc config show container-name | less`

# Editing profile and mentioning memory size
`lxc profile edit custom`

# To push file to lxc container
`lxc file push file-name container-name/container-path`

# To pull file from container to host
`lxc file pull container-name/file-path .`

# Taking snapshots of lxc container
# making temp dir's
`for i in $(seq 5); do mkdir $i; done`
`lxc snapshot container-name snapshot-name`

`lxc list`

# To restore lxc container from snapshot
`lxc restore container-name snapshot-name`

# for nested lxc containers security configuration
`lxc config set container-name security.privileged true`
`lxc config set container-name security.nesting true`

