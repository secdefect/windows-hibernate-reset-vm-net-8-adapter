# Windows hibernate wake reset vmnet8 adapter fix Task
Windows Task to disable/enable VMNet8 adapter after hibernate wake

VMware NAT adapter is known to break after a hibernate wake or sleep wake

This task automates running disable/enable as system to get your VM adapter working - so will run whilst you're not yet logged in

# import the task in Windows Task Scheduler
![image](https://user-images.githubusercontent.com/7570041/153467198-aef35eee-7af6-4048-b69f-9e255e43b56e.png)


## import in administrator cmd.exe
```
schtasks /create  /TN "\VMWAREHibernate-ResetVMnet8" /ru "SYSTEM" /xml "%UserProfile%\downloads\VMWAREHibernate-ResetVMnet8.xml"

```
