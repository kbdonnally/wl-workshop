# Outline

*NB: typing up hand-written notes/brainstorming taken on 9/26/18.*

## BIG GOAL: What is the web and how can I participate in it?

- What is a browser actually displaying?
- What's the difference between websites and formatting on, say, a Word document?

### Starting Point

- From handwritten notes: "when I write this, the fuschia ink is part of the sentence. Indelible."
- Digital displays separate the look of what I'm writing from the content.
- HTML = buckets for text
    - Still has some structure, based on how people naturally organize information
        - What kind of structure? Think: things you might include in class notes (e.g. headers, paragraphs, emphasis/underlines, lists, pictures/drawings)
    - Semantic tags also serve as a failsafe in case something goes wrong and no style instructions load
        - "Sematnic" = "like a human"
        - Also important because screen readers = what if your styles *never* loaded? Does your content still make sense? (e.g. can I tell where a section begins and ends?)

- CSS = "paint by numbers" for any chunk of text
    - Tags are important because they're the smallest unit that CSS rules can work off of
    - CSS can see, but it can't read: it has no idea what the text says, so it can't highlight every instance of like, the word "muffin" unless you put tags around the word -> then, it can do so only because you're like "hey highlight this kind of tag in this place"

- JS = li'l helper buddy for when you *do* need to style based on content and can't do so via "paint" rules
    - Also, any "Harry Potter image"-style interaction b/t user and content

- Browser = read and apply all those instructions
    - Every page you see is just a bunch of text that the browser has painted for you

### Acronyms, Decoded

*insert annotated explainers of HTML, CSS, and JS acronyms.* (Exist hand-written but gonna have to digitize with iPad/Apple Pencil b/c very Not Text Friendly -> webpages can't easily handle everything yet!!! :))

### What's in a webpage?

- HTML = necessary
- CSS = optional, but present >99% of time
- JS = optional, use if need to
    - Don't worry about frameworks; they all compile into plain HTML/CSS/JS, so if you master those, everything else is icing on cake and is way easier to learn

- Literally everything on the web is made out of these 3 ingredients (plus pics, but those get embedded in HTML)

## Other Thoughts

1. Explain how to read HTML and attribute meanings
2. Your preferred setup for CSS
3. HTML document structure
4. Google Fonts
5. Filepaths and filenames/directory names
6. Block vs. inline display
7. CSS Grid/Flexbox
    - Unsure if too hard but it's *so* important, re. easily doing complicated things.
8. Command line, decoded
9. JS "hello, world"
10. DOM and developer tools
11. Jekyll and site generators
    - Plus concept of server in that context, I guess? Don't get too weeds-y on this though
12. Git???
13. Markdown and Markdown Chrome extension
    - View rendered files in browser instantly with no local server
14. File structure of a website
15. Let's make a Jekyll page
    - DIY Wikipedia page, styled however we want
    - Everyone picks person of choice -> good place to have individual decision-making, plus variety of content (images, text, links, headers, sidebars, lists) that stays the same across all pages (e.g. birthday)