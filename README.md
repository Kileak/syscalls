# syscalls
Show syscall information for different architectures.

Just a short script, which eases the pain searching for syscalls and the corresponding registers.

Just clone it, and probably add the directory to $PATH to have it easily accessable.

```
Usage: syscalls <arch> <syscall name / syscall number>
```

```
syscalls x86 execve

#               : 11
Name            : execve
eax             : 0x0b
ebx             : const char *name
ecx             : const char *const *argv
edx             : const char *const *envp
esi             : -
edi             : -
ebp             : -
Definition      : arch/x86/kernel/process.c

syscalls arm read

#               : 9437187
Name            : read
r7              : 0x900003
r0              : unsigned int fd
r1              : char *buf
r2              : size_t count
r3              : -
r4              : -
r5              : -
Definition      : fs/read_write.c
```