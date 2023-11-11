## Over The Wire

I'm practicing Capturing the flag in `OverTheWire - Bandit`, Here, they hide 
the password in somewhere, and we need to find it with 
our technical skills. I'm uploading my level completion here

Level 1 - `NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL`

Level 2 - `rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi`

Level 3 - `aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG`

Level 4 - `2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe`

Level 5 - `lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR`

bandit 6 - `P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU` - find ./ -type f -size 1033c ! -executable

bandit 7 - `z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S` - find / -user bandit7 -group bandit6 -size 33c -type f | grep -i "password" 

Located in : /var/lib/dpkg/info/bandit7.password 

bandit 8 - `TESKZC0XvTetK0S9xNwm25STk5iWrBvP` - grep "millionth" data.txt

bandit 9 - `EN632PlfYiZbn3PhVK3XOGSlNInNE00t` - sort data.txt | uniq -u

bandit 10 - `G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s` - strings data.txt (looks like a flag, just tried it)

bandit 11 - `6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM` -echo -n "encodedString" | base64 -d (for decoding)

bandit 12 - `JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv` (used rot13.com to rotate characters)
