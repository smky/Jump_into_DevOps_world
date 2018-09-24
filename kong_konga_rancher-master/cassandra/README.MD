# Setup Cassandra database

## With rancher-nfs

### Setup guide
```
sudo apt-get update
sudo apt-get install nfs-kernel-server
sudo mkdir /nfs
sudo chown nobody:nogroup /nfs
```
#edit file /etc/exports
```
/nfs    *(rw,sync,no_subtree_check,no_root_squash)
```
```
sudo systemctl restart nfs-kernel-server
```

and setup rancher-nfs at Rancher control panel



