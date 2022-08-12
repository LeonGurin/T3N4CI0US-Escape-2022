# WHISEN

**100 points**

You'd hate to combine.

_Given:_ [prob-011445]()

___

**Was not solved by me, but was solved by my teammate**

Like `Warmup` my teammate was faster (:

Using `ltrace` on the file and entering a nonsense string gives us the `strncmp` function and the strings it compares with.

The first string compared with in the function is `T3N4CI0US{r00T_f0r_h4ck3r\023\255d/V`.

The weird slash characters that come after the word `h4ck3r` change with each run of the program and thus I concluded that they cannot be part of the flag.

I copied the string and added the closing curly brace and that was the flag:

>T3N4CI0US{r00T_f0r_h4ck3r}