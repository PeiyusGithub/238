#### Inrerlude: Process API

**fork()**  
the fork() system call, create a copy of current process: child and parent(original process)  
they both execute the code next to  line fork(), unordered.   
fork return value | meaning
------|---
negative| error
0|child
positive|parent, and the value is child pid

getpid() return current process's id

**wait ()**  
the wait() keeps waiting until child process finish, it does not matter when the parent process execute, it has to wait for the child first.

**exec()**   
exec() does not create a new process, rather, it transforms the currently running program into a different running program

**redirection**: the output of one process seamlessly used as input to the next.
