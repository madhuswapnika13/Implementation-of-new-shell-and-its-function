# Implementation-of-new-shell-and-its-function

The main purpose of this project is that we make our own shell script and include our own
functions into it. We have used C code program for implementing shell and its functions. The
main functions that we have coded are listed as below:

 cddir – Change Directory
 help – Lists down implemented functions
 wipe – clears the screen
 makedir – creates directory
 sysdate – displays current system data and time
 open – opens a file
 copy – copies a file
 delete – deletes a file
 deldir – deletes a particular directory
 rname – renames the file
 cwd – returns current working directory
 list – returns a list of all directories
 hist – returns command history
 file – creates a file
 exit – exits the shell
 virstat – virtual memory statistics
 cpu – display cpu information and architecture
 cpuusage – reports processor related statistics
 statio – input/output statistics for devices and partitions
 process – display user processes
 meminfo – shows RAM usage
 interr – shows number of interrupts
 dskmem – shows disk space usage
 iptraf – IP LAN monitor
 version – displays the version of OS
 memfrag – used to identify memory fragmentation issues
 iomem – system memory for every physical address
 locks – displays files locked by the kernel
 calender–displays the calendar of the current month
 factor–displays the factors of a number
 export–set environment variable
 unset–unset environment variable
 jobs–list all current jobs
 fg–put a job to foreground

 bg–put a job to background
 kill–kill a job
Implementing a self-created Unix Shell in C. By creating this shell, we can add various
functions of our choice and make the shell as versatile as possible. The lifetime of a shell is
quite simple and can be explained in three main terms:
 Initialize: In this step, a typical shell read and execute its configuration files. These
changes aspects of the shell’s behavior.
 Interpret: Next, the shell reads commands from stdin (which could be interactive, or
a file) and executes them.
 Terminate: After its commands are executed, the shell executes any shutdown
commands, frees up any memory, and terminates.
 We are actually going to use them for the basis of our shell. Our shell won’t have any
configuration files, and there won’t be any shutdown command. We can just call the
looping command and terminate later on.
 The first few lines are just declarations and then using do-while looping because it is
more convenient for checking status variable, we check the value once before
executing.
