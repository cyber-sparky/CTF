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

While Solving the level 3, level3 executable file is using strcmp() method compares two string in c language i guess, i used ltrace command to see whats happening in there ! interesting I was able to see the source code and came to know about what string it is comparing, Its comparing string 'snlprintf', and i tried and got into the machine and got the password in the directory /etc/leviathan_pass/leviathan4

- level 4 - `AgvropI4OA`

When I entered in this level there's nothing the home directory, then i started exploring is there any hidden files, and interestingly there's a folder 'trash'. Inside that there a executable file named bin, I cat the file its binary file. when I used ltrace.

<img width="413" alt="image" src="https://github.com/cyber-sparky/CTF/assets/85377859/1cc4b532-4cfa-44c0-8b40-bd817387ddf1">

It's actually reading the password file. when i normally ran the file, it gave me same binary files and i went google searched some binary to text converters. Successfully I am able to find the answer 

- level 5 - `EKKlTF1Xqs`

In this level, there a executable file named `leviathan5` and  when i run its reading a file in /tmp/file.log, But theres no file in /tmp, eventually there's no permission for listing the files in /tmp directory. then i started thinkng is there's any other way, roaming around, then i came back and thinking again, there's no file in /tmp, why wouldn't I create one!. Whats next !? Yeah linking the password file to this file, Used symbolic link to do this. After successfully linking i ran the same file again and I got the answer..!

- level 6 - `YZ55XPVk2l`
