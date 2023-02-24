# to list all the lxc profiles
`lxc profile list`

# to print details of specific profile
`lxc profile show default`

# copying default profile
`lxc profile copy default custom-profile`

# launching container with profile
`lxc launch ubuntu:16.04 myUbuntu --profile=custom-profile`

