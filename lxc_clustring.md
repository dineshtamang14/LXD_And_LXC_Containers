# In order to create a lxc cluster, cluster should be initize during the initial process.
`lxd init`

# listing a lxc cluster
`lxc cluster list`

# in slave node
`sudo lxd init`

# To print details of cluster
`lxc cluster show cluster-name`

# Launching a container in cluster 
1. without target by default
`lxc init ubuntu:16.04 container-name`

2. with target
`lxc init ubuntu:16.04 container-name --target node-name`

# Listing a lxc Network
`lxc network list`

# printing a detail of over laying network 
`lxc network show lxdfan0`

# Editing the network
`lxc network edit lxdfan0`