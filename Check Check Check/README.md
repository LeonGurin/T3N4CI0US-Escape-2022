# Check Check Check

**50 points**

mic test one, two, three!!!

IP : 34.64.203.138
Port : 10009

___

I was bitter about this challenge because for the longest time it didn't work.

When it finally decided to work for me, I connected to the challenge with:
> nc 34.64.203.138 10009

and this gets us a shell.

Navigating through random directories like temp and seeing a community file named `lol` I because inspired and created my own: `lol2`.

Anyways the flag was in:
`/home/ctf/` in a file promplty named `flag`.

catting it gives us:

>T3N4CI0US{ZG9yb3Jvbmc/ZG9uZz9kaW5nPw}
