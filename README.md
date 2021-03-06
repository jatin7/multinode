# multinode
This is to create multiple virtual machines using vagrant script

# Reference video
* We have demonstrated as part of video in YouTube channel
* You can watch the video from this [blog post](https://kaizen.itversity.com/courses/linux-fundamentals-for-software-professionals/lessons/session-11-setup-virtual-environment-using-virtual-box-and-vagrant/)


# Instructions
* Clone the repository
* Make necessary changes to manifest.yml
* It can create up to 10 virtual machines
* Here are the default settings in manifest.yml
```
---
  instances: 6
  name_prefix: pvc00 
  memory: 8192
  cpus: 2
  privateip_prefix: 192.168.100.21
  bootstrap: bootstrap.sh
```
* This will create 6 virtual machines from 192.168.100.210 to 192.168.100.215
* Each virtual machine is of size 8 GB memory and 2 CPUs
* Each virtual machine will be created with 2 virtual hard drives which can expand up to 60 GB each
* Values related to virtual hard drives are hardcoded and hence make sure to understand side effects if you use to create them on local PC. 
