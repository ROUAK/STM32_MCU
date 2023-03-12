

https://user-images.githubusercontent.com/50242654/224540451-7b3afca7-6108-4f5c-879d-d4e5657f784a.mp4

OpenOCD Debugger and Semi-hosting
======================================
Set the linker arguments 
-specs=rdimon.specs -lc -lrdimon

Add semi-hosting run command
monitor arm semihosting enable 

Add the below function call to main.c 
extern void initialise_monitor_handles(void);
initialise_monitor_handles();
