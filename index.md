## Assignment 5.2 — CSS Selectors Practice

### File 1: `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Selectors Practice</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1>CSS Selectors Practice</h1>

    <p>This webpage demonstrates different CSS selectors.</p>

    <section id="intro">
        <h2>Introduction</h2>
        <p>CSS selectors help us style HTML elements.</p>
    </section>

    <section class="card">
        <h2>Element Selector</h2>
        <p>This is the first card.</p>
    </section>

    <section class="card">
        <h2>Class Selector</h2>
        <p>This is the second card.</p>
    </section>

    <section class="card">
        <h2>CSS Practice</h2>
        <p>This is the third card.</p>
    </section>

    <p class="highlight">This paragraph demonstrates cascade and specificity.</p>

</body>
</html>
```

### File 2: `style.css`

```css
* {
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    color: #333333;
}

h1 {
    color: navy;
}

p {
    font-size: 16px;
}

.card {
    background-color: white;
    padding: 15px;
    margin: 10px;
    border: 1px solid gray;
}

#intro {
    background-color: lightblue;
    padding: 15px;
}

h2, p {
    font-family: Arial, sans-serif;
}

.highlight {
    color: blue;
}

p.highlight {
    color: red;
}
```

### Short Explanation of Selectors

1. **Element Selector:** `h1` and `p` style all matching headings and paragraphs.
2. **Class Selector:** `.card` styles multiple sections with the same class.
3. **ID Selector:** `#intro` styles the specific introduction section.
4. **Universal Selector:** `*` applies `box-sizing: border-box` to all elements.
5. **Grouping Selector:** `h2, p` applies the same font family to headings and paragraphs.
6. **Cascade and Specificity:** `.highlight` sets the text color to blue, but `p.highlight` sets it to red because it has higher specificity. Therefore, the highlighted paragraph appears red.
7.