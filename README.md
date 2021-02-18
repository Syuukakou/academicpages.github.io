Person Acamedic Page

ToDoList:
1. access Windows Host Shared folder from VMware Ubuntu
- mount the shared folder
<br> `sudo vmhgfs-fuse -o allow_other .host:/ /mnt/hgfs`
- unmount the shared folder
  <br> `sudo unmount /mnt/hgfs`
  <br> if `umount: /mnt/hgfs: target is busy`
    1. check the folder is used or not (even if you are in the folder used `cd` )
     <br>`sudo fuser -mnv /mnt/hgfs`
  
