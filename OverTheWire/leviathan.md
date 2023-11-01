## Leviathan

- level 0 - `leviathan0`
- level 1 - `PPIfmI1qsA`
- level 2 - `mEh5PNl10e`

While Solving in the level 2, At first I don't have any idea about this level. Then there's a executable file called printfile,
then i try to print the `/etc/leviathan_pass/leviathan3`, it says "You cant have that file... " and I surfed google and I came to know about 'ltrace' and 'strace',

```bash
$ ltrace ./printfile /etc/leviathan_pass/leviathan3
__libc_start_main(0x804852b, 2, 0xffffd764, 0x8048610 <unfinished ...>
access("/etc/leviathan_pass/leviathan3", 4)                         = -1
puts("You cant have that file..."You cant have that file...
)                                  = 27
+++ exited (status 1) +++
```
The access method is doing something in this code, then i try to create a file and make symbolic link, Initially I don't have write access, then i tried creating a file /tmp and make symbolic link and printed the file and yeah! I got the answer.

- level 3 - `Q0G8j4sakn`



