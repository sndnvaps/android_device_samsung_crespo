#CRESPO4G | Nexus 4g | samsung sph-d720 


## i had convert the /sdcard from vfat to ext4

when flash the ubunt touch (phablet-saucy) to the device 
you'd better add the below to '/etc/fstab'

```
#command 
adb shell
echo '/dev/mmcblk0p1  /system    ext4    noatime,nodiratime      0       0' >> /etc/fstab
echo '/dev/mmcblk0p2   /sdcard   ext4    rw                      0       0' >> /etc/fstab
```

#Need to do ,
fix graphics 
EGL not working 
sensorservice not working


