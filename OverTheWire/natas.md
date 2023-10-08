- Level 1: `g9D9cREhslqBKtcA2uocGHPfMZVzeFK6`
- Level 2: `h4ubbcXrWqsTo7GGnnUMLppXbOogfBZ7`
- Level 3: `G6ctbMJ5Nb4cbFwhpMPSvxGHhQ7I6W8Q`
- Level 4: `tKOcJIbzM4lTs8hbCmzn5Zr4434fGZQm`

## Challenge faceed at natas4
At Level 4 i got stuck and i don't have any idea of solving this problem. I googled for long time. Then i discovered a new concept `referer`,

`The Referer is an HTTP header field that identifies the address of the webpage that linked to the resource being requested. When you click a link on a webpage, your browser includes the Referer header in the request sent to the new page. This header provides the URL of the page from which the request originated.`

I found how to solve the problem, There are many ways we can solve this problem:
- Owasp zap
- Burp suite
- Header editor extension

Attempt 1:
I tried installing `zap` but I don't have admin previlege, i tried in my dad's computer which is a 32-bit operating system. `zap` required java 11 to run zap. I tried to downloading java 11 for 32-bit operating system. But i came to know about that java stopped providing 32-bit operating system after `java 8`. Due to that this case failed ☹

Attempt 2:
I tried installing burp suite in my dad's computer. Burpsuite require 64-bit to run burpsuite, then i tried searching burpsuite portable version, it nowhere found in the internet. This case also failed ☹

Attempt 3:
I tried installing varies header editor extensions in chrome, firefox and none of them worked properly. Then i found [Referer Control](https://chrome.google.com/webstore/detail/referer-control/hnkcfpcejkafcihlgbojoidoihckciin), Initially i dont have any idea of using this, then i surfed youtube like 30min, then i got little knowledge of how its working. Then i tried after a day. its working properly. 

- Level 5 : `Z0NsrtIkJoKALBCLi5eqFfcRN82Au2oD`

  
