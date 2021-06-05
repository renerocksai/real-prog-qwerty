# Real Programmer's QWERTY



# Motivation 
Inspired by ThePrimeagen's [Real Programmers Dvorak](https://github.com/ThePrimeagen/keyboards), I realized my QWERTY layout needs an update, too.

But let the harpoon man speak for himself:

> I type everyday of the week. For five of those seven days, i type for about 6-7 hours. It makes sense, removing my will for complacency, that i switch to a more efficient keyboard, if there is one. I present to you, Real Programmers Dvorak.

While I wouldn't go full dvorak myself, the rest of it makes perfect sense, especially after switching to a [Kinesis Advantage 2](https://kinesis-ergo.com/keyboards/advantage2-keyboard/) keyboard, where it's all about comfy programming now :-)!



## The idea of going full-programmer layout

In short:

1. Symmetrical symbol layout (parens, brackets, curlies)
2. Removing the need for SHIFT by putting numerical digits on the SHIFT row instead

The main idea for me was a good symbol layout with the main focus being on a somewhat symmetrical layout of opening and closing braces, brackets, and parentheses. That means, the finger used to close is the same finger on the other hand, like: left index finger for opening parens, right index finger for closing parens.

The second idea was, having those symbols accessible without needing to press the SHIFT key. Intuitively it made sense immediately that I type numbers far less frequently than I type those brackets, parens, and curly braces. And pressing SHIFT+1 instead of 1 is really not a big deal. 



## Implementing it
Since parens are already present on the number row, only four symbols have to be replaced to make space for brackets and curly braces. Regarding placement, all of the opening and closing symbols must be easily accessible for me. On my keyboard that means, using 2, 3, 4 and 7, 8, 9 keys which are reachable easily by extending my ring, middle, and index fingers.

So this boils down to the following mapping:

- 2 - `[` 
- 3 - `{`  
- 4 - `(`
- 7 - `)`
- 8 - `}`
- 9 - `]`

Eventually, I decided on which symbols to move off the number row:

- @ - goes right below the redundand key below the X (`\` / `|`) + SHIFT
- % - also goes below that redundand key, un-shifted
- & - goes where [ was
- ! - goes where ] was

This results in the following re-mapping of the top-row:

LEFT:
- <key>=</key> - <key>=</key>
- <key>1</key> - <key>*</key>
- <key>2</key> - <key>[</key>
- <key>3</key> - <key>{</key>
- <key>4</key> - <key>(</key>
- <key>5</key> - <key>#</key>

RIGHT:
- <key>6</key> - <key>^</key>
- <key>7</key> - <key>)</key>
- <key>8</key> - <key>}</key>
- <key>9</key> - <key>]</key>
- <key>0</key> - <key>$</key>
- <key>-</key> - <key>-</key>

The numerical digits 0-9 are accessible by pressing the SHIFT key and the respective number key.


# Installing it

These instructions have been tested on Ubuntu 20.04 LTS.

- clone this repository and cd into it
- link the layout into the right place: `sudo ln -s /usr/share/X11/xkb/real-prog-qerty real-prog-qwerty`
- activate the layout by `setxkbmap -layout real-prog-qwerty`
- revert it by invoking `setxkbmap -layout us` (provided you were using a US layout before)

If I am feeling funny, maybe one day I will look at ThePrimeagen's repo and check out how to do this on Windows. To be honest, though, optimizing for productivity AND using Windows doesn't strike me as a good combination.

## A note on i3
The best part of this is that I did not have to change my i3 config at all. i3 handles keyboard events directly, so $mod+SHIFT+1 keeps working as expected.



