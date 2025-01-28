# HTML: A to Z

HTML (HyperText Markup Language) is the standard language for creating webpages and web applications. Below is a comprehensive guide to HTML, from the basics to advanced concepts.

---

## Table of Contents

1. [What is HTML?](#what-is-html)
2. [HTML Basics](#html-basics)
3. [HTML Structure](#html-structure)
4. [Common HTML Tags](#common-html-tags)
5. [HTML Attributes](#html-attributes)
6. [HTML Forms](#html-forms)
7. [HTML Tables](#html-tables)
8. [HTML Multimedia](#html-multimedia)
9. [HTML Semantics](#html-semantics)
10. [HTML APIs](#html-apis)
11. [HTML Best Practices](#html-best-practices)
12. [HTML Accessibility](#html-accessibility)
13. [Useful Resources](#useful-resources)

---

## What is HTML?
HTML is the backbone of the web, used to define the structure and content of a webpage. It works alongside CSS (for styling) and JavaScript (for interactivity).

Key points:
- HTML stands for HyperText Markup Language.
- It uses elements to define content.
- It is not a programming language but a markup language.

---

## HTML Basics

### Elements and Tags
- **Tags**: Define elements in HTML. Example: `<p>` for a paragraph.
- **Elements**: Consist of opening and closing tags and the content between them.
  ```html
  <p>This is a paragraph.</p>
  ```

### Doctype Declaration
Defines the HTML version. Example:
```html
<!DOCTYPE html>
```

### Comments
Add comments to describe code:
```html
<!-- This is a comment -->
```

---

## HTML Structure
Basic structure of an HTML document:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Welcome to HTML</h1>
    <p>This is a sample webpage.</p>
    <script src="script.js"></script>
</body>
</html>
```

---

## Common HTML Tags

### Headings
Headings range from `<h1>` (most important) to `<h6>` (least important):
```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
```

### Paragraphs and Text Formatting
```html
<p>This is a paragraph.</p>
<strong>Bold Text</strong> <em>Italic Text</em>
<mark>Highlighted Text</mark> <small>Small Text</small>
```

### Lists
#### Ordered List:
```html
<ol>
    <li>First Item</li>
    <li>Second Item</li>
</ol>
```

#### Unordered List:
```html
<ul>
    <li>First Item</li>
    <li>Second Item</li>
</ul>
```

### Links and Images
```html
<a href="https://example.com" target="_blank">Visit Example</a>
<img src="image.jpg" alt="Description of image">
```

---

## HTML Attributes
Attributes provide additional information about elements. Example:
```html
<a href="https://example.com" target="_blank">Open in new tab</a>
<img src="image.jpg" alt="Description">
```
Common attributes:
- `id`: Unique identifier for an element.
- `class`: Groups elements for styling.
- `style`: Inline CSS styling.
- `title`: Adds a tooltip when hovering.
- `data-*`: Custom data attributes.

---

## HTML Forms
Forms collect user input:
```html
<form action="submit.php" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">
    <button type="submit">Submit</button>
</form>
```

Input types include:
- `text`, `password`, `email`, `number`, `date`, `radio`, `checkbox`, `file`, etc.

---

## HTML Tables
Tables organize data:
```html
<table border="1">
    <thead>
        <tr>
            <th>Name</th>
            <th>Age</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>John</td>
            <td>30</td>
        </tr>
        <tr>
            <td>Jane</td>
            <td>25</td>
        </tr>
    </tbody>
</table>
```
Additional tags:
- `<caption>`: Adds a title to the table.
- `<colgroup>`: Defines column groups for styling.

---

## HTML Multimedia

### Audio
```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

### Video
```html
<video controls width="600">
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video element.
</video>
```

### Embedding Media
```html
<iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
```

---

## HTML Semantics
Semantic tags provide meaning to the content:
- `<header>`, `<footer>`, `<article>`, `<section>`, `<aside>`, `<main>`

Example:
```html
<main>
    <article>
        <h1>Article Title</h1>
        <p>Article content goes here.</p>
    </article>
</main>
```

---

## HTML APIs
Modern HTML provides APIs for advanced features:
- **Geolocation**:
  ```html
  <button onclick="getLocation()">Get Location</button>
  <script>
      function getLocation() {
          if (navigator.geolocation) {
              navigator.geolocation.getCurrentPosition(position => {
                  console.log(position.coords.latitude, position.coords.longitude);
              });
          }
      }
  </script>
  ```
- **Canvas**:
  ```html
  <canvas id="myCanvas" width="200" height="100" style="border:1px solid #000;"></canvas>
  <script>
      const canvas = document.getElementById('myCanvas');
      const ctx = canvas.getContext('2d');
      ctx.fillStyle = 'blue';
      ctx.fillRect(20, 20, 150, 75);
  </script>
  ```

---

## HTML Accessibility
Accessibility ensures your website is usable by everyone, including people with disabilities.

### Tips for Accessible HTML:
1. Use semantic elements (e.g., `<header>`, `<main>`).
2. Add `alt` attributes to images.
3. Use labels for form elements:
   ```html
   <label for="email">Email:</label>
   <input type="email" id="email" name="email">
   ```
4. Ensure sufficient color contrast.
5. Provide keyboard navigation support.
6. Use ARIA (Accessible Rich Internet Applications) roles and attributes where needed.

---

## HTML Best Practices
- Use semantic tags for better accessibility.
- Validate your HTML with tools like [W3C Validator](https://validator.w3.org/).
- Keep your code clean and readable.
- Optimize images and media for faster load times.
- Use meta tags for better SEO:
  ```html
  <meta name="description" content="A comprehensive guide to HTML.">
  <meta name="keywords" content="HTML, Guide, Tutorial">
  <meta name="author" content="Your Name">
  ```

---

## Useful Resources
- [HTML MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [W3Schools HTML Tutorial](https://www.w3schools.com/html/)
- [HTML Living Standard](https://html.spec.whatwg.org/)
- [A11y Project (Accessibility)](https://www.a11yproject.com/)

---

Happy Coding! 
# Author
[Shiful Islam Shohag](https://www.linkedin.com/in/shiful-shohag/)
