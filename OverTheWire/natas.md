## Natas Challenges Progress:

- **Level 1:** `g9D9cREhslqBKtcA2uocGHPfMZVzeFK6`
- **Level 2:** `h4ubbcXrWqsTo7GGnnUMLppXbOogfBZ7`
- **Level 3:** `G6ctbMJ5Nb4cbFwhpMPSvxGHhQ7I6W8Q`
- **Level 4:** `tKOcJIbzM4lTs8hbCmzn5Zr4434fGZQm`
- **Level 5:** `Z0NsrtIkJoKALBCLi5eqFfcRN82Au2oD`

---

## Challenge Faced at Natas Level 4:

Upon reaching Level 4, I encountered a roadblock and was clueless about solving the problem. After extensive research, I stumbled upon a vital concept: the **Referer** header.

### Understanding the Referer Header:

The **Referer** header is an HTTP field that reveals the address of the webpage linking to the requested resource. Essentially, when a link is clicked, the browser includes the Referer header in the request, indicating the originating page's URL.

### Solution Exploration:

My initial attempts involved using various tools like **Owasp Zap**, **Burp Suite**, and header editor extensions to manipulate the Referer header. However, each endeavor posed unique challenges:

- **Attempt 1:** I attempted to use **Owasp Zap**, but I faced limitations due to lacking admin privileges. Additionally, my dad's computer, equipped with a 32-bit operating system, couldn't support the required Java 11 version.

- **Attempt 2:** Installing **Burp Suite** presented another hurdle; it demanded a 64-bit system, leading me to search for a portable version without success.

- **Attempt 3:** Turning to browser extensions, I experimented with various header editor extensions for Chrome and Firefox, but none proved effective. After hours of searching, I discovered the **Referer Control** extension. Initially unfamiliar with its workings, I delved into YouTube tutorials, gaining insights after roughly 30 minutes of research. Armed with newfound knowledge, I made a successful attempt the following day.

With these experiences, I overcame Level 4 and proceeded to Level 5, where the challenge continued.

- **Level 5:** `Z0NsrtIkJoKALBCLi5eqFfcRN82Au2oD`
- **Level 6:** `fOIvE0MDtPTgRhqmmvvAOt2EfXR6uQgR`
- **Level 7:** $secret = FOEIUWGHFEEUHOFUOIU - `jmxSiH3SP6Sonf8dv66ng8v1cIEdjXWr`
- **Level 8:** `a6bZCNYwdKqN5cGP11ZdtPg0iImQQhAB`
- **Level 9:** after compiling given function - oubWYf2kBq - `Sda6t0vkOPkM8YeOZkAGVhFoaplvlJFd`
- **Level 10:** `D44EcsFkLxPIkAAKLosx8z3hxX1Z4MCE`

### Learning in natas 9

Everything we do in hacking/exploitation is interconnected, `EVERY INFORMATION IS VALUABLE`.
After seeing natas 9 source code, i came to know about that this can be exploited by `Command Execution`, The value of `$_REQUEST["needle"]` is used directly in the `passthru()` function without validation or sanitization, allowing an attacker to manipulate the input to execute arbitrary commands. Then tried `; ls -la`, its listing the files which are present in the directory. In the previous challenge and when initially starting this natas challenge they mentioned `All passwords are also stored in /etc/natas_webpass/.` and ran `; cat etc/natas_webpass/natas10` command and Yeah ! i got the flag for next level

- **Level 11:** `1KFqoJXi6hRaPluAmk8ESDW4fSysRoIg` - command i used : `.* /etc/natas_webpass/natas11`
