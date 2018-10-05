---
title: Code Blocks
layout: plain
permalink: /code-blocks/
---

# Code Blocks

## HTML intro slide

- Pic: 03-html
- Code:

{:.language-html}
```
<html>
<head>
    <title>This Displays on Browser Tab</title>
    <link rel="stylesheet" href="link/to/css-styles.css">
    <!-- or, can write CSS in a style element: -->
    <style></style>
</head>
<body>
    <!-- syntax: <tagname>Content!</tagname> -->
    <h1>Biggest text, usually page title</h1>
    <p>Paragraph! Lorem ipsum dolor sic amet...</p>
    <ul>
        <li>List item</li>
        <li>This is in an unordered list</li>
        <li>Aka, one with bullets instead of numbers</li>
    </ul>

    <!-- some tags don't need to be closed -->
    <img src="link/to/pic.jpg" alt="Image description">
    <a href="https://website-url.com">

    <!-- tags also denote page sections -->
    <footer>
        <h2>Footer label</h2>
    </footer>
</body>
</html>
```

- Pic: 07-read-html
- Code:

{:.language-html}
```
<h1 class="page-title">About</h1>
<main>
    <h2 class="page-subtitle">Subtitle</h2>
    <img src="dogs.jpg" alt="Dogs">
</main>
```

- Pic: 08-selectors
- Code 1:

{:.language-html}
```
<body>
    <header>
        <h1>Page Title</h1>
        <h2>What the page is about</h2>
    </header>
    <main>
    ...
    </main>
</body>
```

- Code 2:

{:.language-scss}
```
// HTML   --> CSS
   class  --> .class
   id     --> #id
   <tag>  --> tag
```

- Pic: 09-website-files

- Code:

{:.language-bash}
```
site/
    assets/
    |   css/
    |   |   > style.css
    |   |
    |   |
    |   img/
    |   |   > dogs.jpg
    |   |   > llamas.jpg
    |   |
    |   js/
    |       > main.js
    |
    pages/
    |       > about.html
    |       > contact.html
    |       > work.html
    > 404.html
    > index.html
    > favicon.ico
```

- Pic: 13-mockup-to-html
- Code - actual HTML:

{:.language-html}
```
<div class="about-wrapper">
    <header class="about-header">
        <h1 class="abt-head__page-title">About</h1>
    </header>
    <main class="about-main-content">
        <section class="about__origins">
            <h2 class="about-origin__title">Blah</h2>
            <p>Lorem ipsum dolor blah</p>
            <div class="about-origin__pic">
                <img src="pic.jpg" alt="pic">
                <span>Caption for image</span>
            </div>
        </section>
        <section class="about__our-work">
        ...
        </section>
    </main>
</div>
```

{:.language-ruby}
- Code - fake HTML:
    ```
    <page title>

    <section 1>
        <title>
        <p>
        <pic>
            <img>
            <span>
        </pic>
    </section 1>

    <section 2>
        <title>
        <content>
            <p>
            <ul>
            <p>
        </content>
    </section 2>
    ```

- Pic: 12-mockup-to-css

Info:

{:.language-css}
- CSS prefix: `about-`
- Structure: `.prefix-parentblock__purpose--type`
- Example:
```
.about__section1 { ... }
.about-sec1__title { ... }
.about-sec1__content { ... }
.about-content__pic { ... }
.about-content__pic img { ... }
.about-content__pic span { ... }
```