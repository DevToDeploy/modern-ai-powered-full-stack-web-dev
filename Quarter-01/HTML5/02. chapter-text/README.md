# 📘 HTML5 Text and Markup – Chapter 2 Guide

This guide explains **HTML5 text formatting and markup elements** in a clear, beginner-friendly way.  
By reading this, students will understand **what each tag does**, **why it’s used**, and **how to implement it** in real-world web development.

---

## 🧩 What is Text Markup in HTML?

When creating a web page, you use **tags (markup)** to give meaning to text.  
These tags help browsers display content properly and help developers organize information clearly.

There are two main types of markup in HTML:

1. **Structural Markup** – Defines the structure of a document (headings, paragraphs, line breaks, etc.).
2. **Semantic Markup** – Adds meaning to the text (emphasis, citations, definitions, quotes, etc.).

---

## 🏗️ Structural Markup

### 1. Headings: `<h1>` to `<h6>`
Headings create the outline of your web page, like titles and sub-titles in a book.

| Tag | Purpose | Example |
|-----|----------|----------|
| `<h1>` | Main page heading | `<h1>Welcome to My Website</h1>` |
| `<h2>` | Section heading | `<h2>About Us</h2>` |
| `<h3>`–`<h6>` | Subheadings | `<h3>Our Team</h3>` |

**Note:** `<h1>` is the largest; `<h6>` is the smallest.  
Browsers automatically style them with different font sizes.

---

### 2. Paragraphs: `<p>`
Used to define a block of text.

```html
<p>This is a paragraph of text.</p>
<p>Each paragraph starts on a new line.</p>
```

Browsers automatically add space between paragraphs for readability.

---

### 3. Bold & Italic Text: `<b>`, `<i>`, `<strong>`, `<em>`

| Tag | Meaning | Example |
|------|----------|----------|
| `<b>` | Makes text **bold** (no extra meaning) | `<b>Important word</b>` |
| `<strong>` | Indicates *important* text | `<strong>Warning!</strong>` |
| `<i>` | Italicizes text (used for technical terms, names, etc.) | `<i>Endeavour</i>` |
| `<em>` | Adds emphasis to words | `<em>Do not forget!</em>` |

**Difference:**  
- `<b>` and `<i>` are for styling.  
- `<strong>` and `<em>` convey *meaning* (semantic).

---

### 4. Superscript & Subscript: `<sup>` and `<sub>`

Used to display text above or below the normal line.

```html
<p>E = MC<sup>2</sup></p>
<p>H<sub>2</sub>O</p>
```

- `<sup>` – Superscript (like exponents, ², ³)  
- `<sub>` – Subscript (like chemical formulas, H₂O)

---

### 5. White Space

Extra spaces or line breaks in HTML **collapse into a single space**.

```html
<p>The moon   is   drifting away.</p>
```
✅ Output: “The moon is drifting away.”

Indentation in code helps readability but doesn’t affect display.

---

### 6. Line Breaks: `<br>` and Horizontal Rules: `<hr>`

- **`<br>`** creates a new line *inside* a paragraph.
- **`<hr>`** creates a horizontal line, separating topics or sections.

```html
<p>Roses are red,<br>Violets are blue.</p>
<hr>
<p>New topic starts here.</p>
```

Both are **empty elements** (no closing tags).

---

## 🧠 Semantic Markup

Semantic tags give **meaning** to your text so browsers, screen readers, and search engines understand it better.

---

### 7. Emphasis & Strong Importance

| Tag | Use | Example |
|------|-----|----------|
| `<em>` | Highlights part of a sentence | `I <em>really</em> like this book.` |
| `<strong>` | Indicates strong meaning or warning | `<strong>Do not touch!</strong>` |

---

### 8. Quotations: `<blockquote>` and `<q>`

| Tag | Purpose | Example |
|------|----------|----------|
| `<blockquote>` | Long quote (usually indented) | `<blockquote>Be the change you wish to see.</blockquote>` |
| `<q>` | Short quote inside text | `<p>He said, <q>Hello!</q></p>` |

You can add a **`cite` attribute** to mention the source:

```html
<blockquote cite="https://en.wikipedia.org/wiki/Winnie-the-Pooh">
  <p>Did you ever stop to think, and forget to start again?</p>
</blockquote>
```

---

### 9. Abbreviations & Acronyms: `<abbr>`

Used to define shortened forms of words.  
Hovering over the text shows the full meaning.

```html
<p><abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
```

> ✅ HTML5 uses `<abbr>` for both abbreviations and acronyms.

---

### 10. Definitions: `<dfn>`

Used when introducing a new term for the first time.

```html
<p><dfn>Black hole</dfn> is a region of space from which nothing can escape.</p>
```

Browsers may show it in italics.

---

### 11. Citations: `<cite>`

Used to reference the title of a creative work (book, film, article, etc.).

```html
<p><cite>The Scream</cite> by Edvard Munch, 1893.</p>
```

Displayed in italics by default.

---

### 12. Address: `<address>`

Used for **author or contact details**.

```html
<address>
  <p><a href="mailto:homer@example.org">homer@example.org</a></p>
  <p>742 Evergreen Terrace, Springfield.</p>
</address>
```

Browsers often render it in italics.

---

### 13. Inserted, Deleted & Strikethrough Text

| Tag | Purpose | Example |
|------|----------|----------|
| `<ins>` | Text that has been added | `<p>It was the <ins>best</ins> day ever.</p>` |
| `<del>` | Text that has been removed | `<p>It was the <del>worst</del> day ever.</p>` |
| `<s>` | Text that is no longer valid (e.g., old prices) | `<p><s>$99</s> Now $49!</p>` |

---

## 🧰 Additional Elements

| Tag | Description | Example |
|------|-------------|----------|
| `<small>` | Displays smaller text | `<small>Copyright © 2025</small>` |
| `<mark>` | Highlights text | `<mark>Important</mark> message` |

---

## 🧩 Complete Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>HTML5 Text Example</title>
</head>
<body>
  <h1>The Story in the Book</h1>
  <h2>Chapter 1</h2>
  <p>Molly had been staring out of her window for about an hour now. On her desk, between copies of <i>Nature</i> and <cite>On The Road</cite>, lay her favorite book.</p>
  <p>She had spent the last ten years in this room under a poster with a quote: <q>Work is the refuge of people who have nothing better to do.</q></p>
  <p>Molly <em>did</em> think she had something better to do.</p>
</body>
</html>
```

---

## 🧾 Summary

✅ **Structural markup** organizes text using headings, paragraphs, and breaks.  
✅ **Semantic markup** gives meaning to text (emphasis, quotes, definitions, etc.).  
✅ Together, they make web pages more **readable, accessible, and SEO-friendly**.
