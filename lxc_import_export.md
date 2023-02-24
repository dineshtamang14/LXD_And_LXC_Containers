# To launch ubuntu container
`lxc init ubuntu:16.04 myubuntu`

# in order to export container to another node
1. create a snapshot
`lxc snapshot container-name snapshot-name`

or to create a snapshot of running container 
`lxc snapshot container-name snapshot-name --stateful`

2. for information
`lxc info container-name`

3. adding a new remote server information
`lxc remote add name-for-remote-server 172.42.42.102`

4. listing remote servers
`lxc remote list`

5. Transferring container to other server
`lxc copy container-name/snapshot-name remote-server-name:container-name`

# removing remote server details
`lxc remote remove remote-server-name`

# another way of transferring container as a image
1. `lxc publish container-name/snapshot-name --alias custom-image-name`

2. `lxc image list`

note: 
`in order export image to other node we have to export image as a tar file`
3. `lxc image export custom-image-name`

4. Transferring tar file to other node
`scp a2140f.tar.gz 172.42.42.201:`

5. In remote server import tar file as a image
`lxc image import a2140f.tar.gz --alias custom-image-name`

6. `lxc image list`

7. creating a container from that image
`lxc init custom-image-name custom-container-name`

8. `lxc list`