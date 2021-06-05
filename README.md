# Real Programmer's QWERTY

## Motivation 
Inspired by ThePrimeagen's [Real Programmers Dvorak](https://github.com/ThePrimeagen/keyboards), I too realized, my QWERTY layout needs an update

But let the man speak himself:

> I type everyday of the week. For five of those seven days, i type for about 6-7 hours. It makes sense, removing my will for complacency, that i switch to a more efficient keyboard, if there is one. I present to you, Real Programmers Dvorak.

While I wouldn't go full dvorak now, it makes perfect sense. Especially after my switch to a [Kinesis Advantage 2](https://kinesis-ergo.com/keyboards/advantage2-keyboard/) keyboard, since it's all about comfy programming now :-)!

### The idea of going full-programmer layout

In short:
1. Symmetrical symbol layout
2. Removing the need for SHIFT by putting numerical digits on the SHIFT row

The main idea for me was a good symbol layout with the main focus being on a somewhat symmetrical layout of opening and closing braces, brackets, and parentheses. That means, the finger used to close is the same finger on the other hand, like: left index finger for opening parens, right index finger for closing parens.

The second idea was, having those symbols accessible without needing to press the SHIFT key. Intuitively it made sense immediately that I type numbers far less frequently than I type those brackets, parens, and curly braces. And pressing SHIFT+1 instead of 1 is really not a big deal. 

### Implementing it
Ich muss nur die 4

Sie muessen, damit sie schoen erreichbar sind, auf folgende Tasten gemappt werden:

- 2 - `[` 
- 3 - `{`  
- 4 - `(`
- 7 - `)`
- 8 - `}`
- 9 - `]`

Dafuer koennen folgende Symbole weichen: 

- @ - kann unter das SHIFT + X 
- % - kann unter das X 
- & - kann auf [ 
- "!" - kann auf ] 

Das ergibt folgende top row

- = - `=`
- 1 - `*`
- 2 - `[`
- 3 - `{`
- 4 - `(`
- 5 - `#`

- 6 - `^`
- 7 - `)`
- 8 - `}`
- 9 - `]`
- 0 - `$`
- - bleibt

## A note on i3
The best part of this is that I did not have to change my i3 config at all. I had been worried that 
Aus ALT + SHIFT + 1 muss dann CTRL + SHIFT + 1 werden
NEIN! Weil i3 anscheinend das keyboard selbst abfragt!


