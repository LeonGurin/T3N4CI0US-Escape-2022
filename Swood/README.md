# Swood

**250 points**

string

_Given:_ [prob-7290f4](https://github.com/LeonGurin/T3N4CI0US-Escape-2022/blob/main/Swood/prob)

___

**Was not solved by me, but was solved by my teammate**

Like `Warmup` my teammate was faster again :D

Running the file, given us a usage prompt. Supplying a dummy string like `aa` gives us `wrong password` prompt.

Using `ltrace` on the file and entering a nonsense string gives us the `strncmp` function and the strings it compares with.

The first string compared with in the function is `da39a3ee5e6b4b0d3255bfef95601890`.

I tried entering this string but it was still wrong. I thought that the compared with string was bigger than the string displayed so I looked around using `strings` and got the following:

```
da39a3eeH
5e6b4b0dH
3255bfefH
95601890H
afd80709H
```

Erasing the `H` at the end got me: 

>da39a3ee5e6b4b0d3255bfef95601890afd80709

Using it on the `prob` file got me the success string.

I copied the string into the flag format and got:

>T3N4CI0US{da39a3ee5e6b4b0d3255bfef95601890afd80709}