# To Rename profile
`lxc profile rename profile-name new-profile-name`

# To get particular configuration from profile
`lxc profile get default limits.cpu`

# To create custom profile
`lxc profile create custom-profile`

# To list profiles 
`lxc profile list`

# To Delete profile
`lxc profile delete profile-name`

# To Copy existing profile
`lxc profile copy profile-name new-profile-name`

# To Edit Profile
`lxc profile edit profile-name`

# To check cpu and memory
cpu: `nproc`
memory: `free -g`

# To set cpu through lxc command
`lxc profile set profile-name limits.cpu 2`
`lxc profile set profile-name limits.memory "2GB"`

# To get profile properties
`lxc profile get profile-name limits.memory`

# To print profile configurations
`lxc profile show profile-name`

# To grep profile applied to container
`lxc info container-name | grep Profiles`

# To Apply custom profile to container
`lxc profile add container-name profile-name`

