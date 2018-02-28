# character-cycle
That thing you see in films where they're supposedly hacking a password. It cycles through each letter until it appears to hit the  character it's looking for. You'll know it when you see it.

The code's commented so it should be straightforward to use. 

### User for?
Don't know. I was thinking about having a website header that was a string of random characters which resolves into a word. Didn't know how to do it. Worked out how to do it. Decided it wasn't a good idea.

You could easily swap out the function that cycles through the characters and replace it with another effect. e.g. changing the colour of each letter in turn.

### It's a visual effect only
It cycles through a set number of characters, then at the end, drops in the character required, so it's cheating. But it looks the part and uses less code than it would if it cycled to the correct character.

The cycle effect runs through ASCII characters, currently starting at '!' and ending in 'Z'. You can change the start and finish characters.

### Different font?
If you don't use a **monospace** font there's likely to be unsightly jiggling as it cycles through characters of different widths. The letterspacing will change when the span wrap is applied and it will change again when the spans are removed at the end.

### Tidy markup
For what it's worth. The text starts off as a string inside an element. Each letter is then wrapped in a span for the duration of the effect. The new text is then rewritten back into the element without the spans. I suspect Google is going to pick up on your original element content though.
