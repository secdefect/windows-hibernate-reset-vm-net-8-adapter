# Windows hibernate wake reset vmnet8 adapter
Windows Task to disable/enable VMNet8 adapter after hibernate wake


# import the task
![image](https://user-images.githubusercontent.com/7570041/153467198-aef35eee-7af6-4048-b69f-9e255e43b56e.png)

## Run as administrator
'''
schtasks /create  /TN "\VMWAREHibernate-ResetVMnet8" /ru "SYSTEM" /xml "%UserProfile%\downloads\VMWAREHibernate-ResetVMnet8.xml"

'''
