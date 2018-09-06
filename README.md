# passphrase
A simple bash script that generates random dictionary-derived password phrases.  

## Arguments

The script takes these arguments three:

* **-c** <*number*>

  Provides *n* groups of passwords.

* **-s**

  Include spaces between all words.

* **-w** <*number*>

  Provides phrases containing *n* number of words.

Here's an example. Feel free to mix and match and use these as passwords. They would be [good passwords](https://xkcd.com/936/). I'm not using any of them. I swear.

```shell
$ passphrase -c 5 -w 4 -s

solvent griffins squirmed flitting
pallor sensibly bolas scab
checkup laurels unclean chargers
juvenile purblind purples stiffest
ignited enters empties rioted

interred limit jaywalks kiloton
plumage woeful design arranged
tushes excepted stript satire
vouch nitpicks balm framers
impelled chattily plies remember

gaiters maim simian palest
cubicle picnic exhumes sandal
diabetic lames rotting detoxing
lowlands andantes allay premiers
sulfides partaken terrible howdy

segment bookies reviled moralist
wiretaps thong bull poky
rebuilt cleaves poverty worsted
sloshed rubrics fumbler phishers
rusk slab frocks bonbons

sudden ardently cramp royalist
warped temerity jeopardy entreat
buildups tiptop ointment pings
spitball dike dreadful char
violent miscue nunnery blinding
```

## To-do

* provide passwords that meet specific lengths to satisfy [bad bank password requirements](https://stackoverflow.com/a/702438) (sadlol)
* boolean arg to boost cardinality and meet requirements: caps, symbols, digits, etc.
* explore integraion with [pass](https://git.zx2c4.com/password-store/), which currently only leverages [pwgen](https://linux.die.net/man/1/pwgen), which, in my opinion, does not succeed at its primary task of being both highly memorable and high-entropy
