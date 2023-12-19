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

bandit 13 - `wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw`

bandit 14 - `fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq`

bandit 15 - `jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt` - (used netcat to connect)

bandit 16 - `JQttfApK4SeyHwDlI9SXGR50qclOAil1` 

bandit 17 - `VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e`

bandit 18 - `hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg`

bandit 19 - `awhqfNnAbc1naukrpqDYcF95h7HoMTrC`

bandit 20 - `VxCazJaVykI6W36BkBU0mJTCM8rR95XT`

In this level we need to create connect which will listen on a particular port. I used `echo "VxCazJaVykI6W36BkBU0mJTCM8rR95XT" | nc -l -p 1234`, then in the second terminal, try to send the request by giving `./suconnect 1234`, this will return the answer

bandit 21 - `NvEJF7oVjkddltPSrdKEFOllh9V1IBcq` 

bandit 22 - `WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff`

bandit 23 - `QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G`

bandit 24 - `VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar`

bandit 25 - `p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d`

bandit 26 - `c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1`

bandit 27 - `YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS`

bandit 28 - `AVanL161y9rsbcJIsFHuw35rjaOM19nR`

bandit 29 - `tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S`

bandit 30 - `xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS`

bandit 31 - `OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt`

bandit 32 - `rmCBvG56y58BXzv98yZGdO7ATVL5dW8y`

bandit 33 - `odHo63fHiFqcWWJG9rLiLDtPm45KzUKy`
