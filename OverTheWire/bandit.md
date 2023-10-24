## Over The Wire

I'm practicing Capturing the flag in `OverTheWire - Bandit`, Here, they hide 
the password in somewhere, and we need to find it with 
our technical skills. I'm uploading my level completion here

Level 0 - `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

Level 1 - `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`

Level 2 - `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG`

Level 3 - `2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe`

Level 4 - `lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR`

bandit 6 - `P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU` - find ./ -type f -size 1033c ! -executable

bandit 7 - `z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S` - find / -user bandit7 -group bandit6 -size 33c -type f | grep -i "password" 

Located in : /var/lib/dpkg/info/bandit7.password 

bandit 8 - `TESKZC0XvTetK0S9xNwm25STk5iWrBvP` - grep "millionth" data.txt

bandit 9 - `EN632PlfYiZbn3PhVK3XOGSlNInNE00t` - sort data.txt | uniq -u
