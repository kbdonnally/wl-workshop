---
title: Slide Notes
layout: workshop
permalink: /slide-notes/
---

*NB: these are typed notes to pair with code blocks & illustrations.*

# Slide 1: Intro

![Hand lettering]({{ 'assets/img/svg/name.svg' | relative_url }}) <!--("")-->

- This styling, as written, is an inherent part of what I wrote. My hand shaped the letters; the ink made the colors.
- So how do I do this on a screen?

- Let's look at *what* was actually written:
    1. Content: "Katherine"
    2. Styles: text color, border info, size, what font we're using

- Digitized text is literally just that: identifying things about a piece of text and figuring out how to write that in a way computers understand.

- It separates the *content* of what you're writing from *how it looks*. (Just like Microsoft Word or PowerPoint.)

- Everything is text! Browsers are just big ole' text readers.

# Slide 2: What's in a webpage?

- Ingredients:
    - HTML = buckets for text
    - CSS = "paint-by-numbers" instructions
    - Browser = paints the text buckets using those instructions

(There's also this thing called "JavaScript," which basically helps people make cool interactions with motion or timing, but we don't need to worry about that at all right now. Things that required JavaScript 5 years ago, like animation, can be done with CSS now because the future is here.)

# Slide 3: [Annotated Definitions]

- Explain what HTML, CSS, and JS actually stand for.

![HTML and CSS acronyms]({{ 'assets/img/svg/acronyms.svg' | relative_url }}) <!--("")-->

# Slide 4: HTML: A Closer Look

- Reading HTML:
    - Tags: buckets so the browser and CSS can read what you mean
    - Attributes: extra information about that tag ("bucket"), e.g. where a link should go
    - Attributes go in the start tag, so you can scan that info without having to read what's inside the tag

- Attributes are also a main way to give CSS instructions on how to paint something
    - This is primarily done with 2 attributes: `id`, and `class`
    - They can be used the same, except `id` is only allowed to show up once on a page, and class can apply to as many elements as you want.
    - Due to this limitation, I usually "color" everything with classes

# Slide 5: CSS: A Closer Look

- Reading CSS:

{:.language-css}
```
selector {
    property: "value";
}
```

- Terms:
    1. Selector: What part of the HTML you want to "paint" with that instruction.
    2. Property: Something about the HTML element - color, capitalization, position, font, size, etc.
    3. Value: Keywords that a given property will accept. (E.g. color would accept "blue", but wouldn't know what to do with "5.7")

*NB: legit no one knows "all" the CSS properties, and especially not all the values those properties can take. There are some you'll find yourself using a lot, but in general, we're all googling "how to make rounded corners with CSS...", not just writing off the top of our heads. (It's "border-radius" :).)*

# CSS Selectors

{:.language-bash}
- You can give CSS instructions with element types (e.g. `h1`, `p`), classes, and IDs.
- Let's translate a piece of HTML to CSS:

{:.language-html}
```
<h1 class="headings" id="my-name">Katherine</h1>
```

To style *all* `h1` elements on a page:

{:.language-css}
```
h1 {
    color: purple;
}
```

To style all elements with the class `headings`{:.language-bash}, even if they're *not* an `h1`{:.language-bash}:

{:.language-css}
```
.headings {
    color: purple;
}
```

To style *specifically that element*, and nothing else on the page:

{:.language-css}
```
#my-name {
    color: purple;
}
```

# CSS Selectors: A Summary

{:.language-scss}
```
// HTML               --> CSS
   class="class-name" --> .class-name
   id="id-name"       --> #id-name
   <tag>              --> tag
```

# Exercise: Style Your Name

- Let's translate the writing from earlier into a digital version.

![Hand lettering]({{ 'assets/img/svg/name.svg' | relative_url }}) <!--("")-->

- Describe the lettering: big, dark gray, blue border, sans-serif...

- Okay, so let's make that happen. Without knowing anything else, we know big letters = `h1` element.

First try:

{:.language-html}
```
<h1>Katherine</h1>
```

Aaand that looks liiiike...

{:.demo}
# Katherine

Hmm. We have some work to do.

# Steps:

## 1. Adding a class

Let's add a class so we don't accidentally make *all* our header elements look like the image.

{:.language-html}
```
<h1 class="my-name">Katherine</h1>
```

Cool. Now it'll only style things with the class `my-name`{:.language-html}.

## 2. Changing the color

CSS has a bunch of [built-in color names](https://www.w3schools.com/colors/colors_hex.asp) from the 90s when the only other option was to put in a HEX code (16-base numbers, which are about as readable as they sound!). 

These are great to use as a beginner, since they're all just literal words:

{:.language-css}
```
.my-name {
    color: darkgray;
}
```

Now we have...

{:.demo.demo--color}
# Katherine

## 3. Changing the font

{:.language-css}
```
.my-name {
    color: darkgray;
    font-family: sans-serif;
}
```

Result:

{:.demo.demo--color.demo--font}
# Katherine

## 4. Adding a border

{:.language-css}
```
.my-name {
    color: darkgray;
    font-family: sans-serif;
    border: 4px solid lightblue;
}
```

Result:

{:.demo.demo--color.demo--font.demo--border}
# Katherine