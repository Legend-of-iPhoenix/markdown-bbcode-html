A few weeks ago, I had the not-so-crazy idea to write a Markdown renderer in JavaScript. This isn't that hard, Markdown is  *designed* to be easily converted into HTML.

Last night, I realized that BBCode is also designed to be turned into HTML and formatting in Markdown is much more concise than BBCode. Maybe I can write posts faster in Markdown!

This is the result of about a hour of work. The converter uses Regular Expressions to match the Markdown formatting in the input text and replace it with the appropriate BBCode and HTML tags. Here's what I have so far:

# Headings
## Subheadings
(The Markdown to HTML lets you how down to h4, but I'm too lazy to add this to the BBCode version)  
~~strikethrough~~  
**bold**  
_italics_  
Inline `code`  
```
Code 
blocks
```

 * lists
 * more list (it joins adjacent list elements appropriately)  

[Links](https://legend-of-iphoenix.github.io/markdown-bbcode-html/)  
Horizontal bars:
***
Images:  
![my avatar](https://avatars0.githubusercontent.com/u/32944537?s=40)

This post was converted from Markdown into BBCode using the Markdown -> BBCode converter! You can see the source code for this post [here](https://github.com/Legend-of-iPhoenix/markdown-bbcode-html/blob/master/post.md)

You can find the converter at [https://legend-of-iphoenix.github.io/markdown-bbcode-html/](https://legend-of-iphoenix.github.io/markdown-bbcode-html/).

---
To-do
 * Block quotes
 * Somehow, colors???
 * Code cleanup
 * Bugfixing, particularly bugs with italics using asterisks.
 * Escaping? Somehow?
 * Nested lists? Somehow?
 * Make generated HTML a bit nicer-looking. (Apply formatting rules)
 * Clean up the actual website (I think jcgter777 is going to help with this)
 * Add support for more advanced Markdown.
 * Potentially convert BBCode to Markdown?
