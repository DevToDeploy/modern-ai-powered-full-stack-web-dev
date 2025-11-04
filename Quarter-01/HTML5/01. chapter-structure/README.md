# 📘 Chapter One – Understanding HTML5 Structure

## 🧭 Table of Contents

1. [Introduction](#introduction)
2. [What is HTML?](#what-is-html)
3. [Structure of a Web Page](#structure-of-a-web-page)
4. [HTML Tags and Elements](#html-tags-and-elements)
5. [HTML Document Example](#html-document-example)
6. [Explaining Each Tag](#explaining-each-tag)
   * [<body> and </body>](#body-and-body)
   * [<p> paragraphs](#p-paragraphs)
7. [Attributes](#attributes)
8. [Creating Your First Web Page](#creating-your-first-web-page)
9. [Viewing Page Source](#viewing-page-source)
10. [Summary](#summary)

---

## 🧩 Introduction

HTML (HyperText Markup Language) is the **standard language used to create web pages**.
It defines the **structure and layout** of a page using special codes called **tags** or **elements**.

Every document on the web from news articles to product pages relies on **structure** to organize content clearly. HTML provides that structure so browsers can display pages properly.

---

## 🌐 What is HTML?

HTML stands for:

* **H** – Hyper
* **T** – Text
* **M** – Markup
* **L** – Language

**HyperText** means you can link from one page to another easily.
A **Markup Language** means it uses special tags to describe the meaning and structure of content.

---

## 🧱 Structure of a Web Page

A well-structured HTML document has three main parts:

1. **DOCTYPE Declaration** tells the browser the type of document.
2. **Head Section** contains meta information about the document.
3. **Body Section** contains the actual content shown to users.

📘 **Example:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chapter-One-Structure</title>
</head>
<body>
  <h1>My First Heading</h1>
  <p>My first paragraph.</p>
</body>
</html>
```

---

## 🏷️ HTML Tags and Elements

Tags act like **containers** that wrap around content and describe its purpose.

* **Opening Tag:** `<p>`
* **Closing Tag:** `</p>`
* **Element:** `<p>My paragraph text.</p>`

**Tip:**
Every HTML element usually has an opening and a closing tag, unless it’s a **self-closing tag** (like `<meta>` or `<img>`).

---
# 🧭 HTML Headings & Paragraph Tags

## 📘 Introduction
HTML provides heading tags `<h1>` to `<h6>` and a paragraph tag `<p>` to define the structure and hierarchy of content on a web page.  
Headings are used to represent titles and subtitles, while the paragraph tag is used for blocks of text.

---

## 🧱 Default Browser Font Sizes

| Tag | Default Font Size | Default Font Weight | Description |
|------|------------------|----------------------|--------------|
| `<h1>` | **32px** | bold | Main page title |
| `<h2>` | **24px** | bold | Section title |
| `<h3>` | **18.72px** | bold | Subsection title |
| `<h4>` | **16px** | bold | Smaller heading |
| `<h5>` | **13.28px** | bold | Minor heading |
| `<h6>` | **10.72px** | bold | Smallest heading |
| `<p>`  | **16px** | normal | Standard paragraph text |

> 🧩 **Note:**  
> These are based on the browser’s default style (base font size = 16px).  
> For example:
> ```css
> h1 { font-size: 2em; }
> h2 { font-size: 1.5em; }
> h3 { font-size: 1.17em; }
> h4 { font-size: 1em; }
> h5 { font-size: 0.83em; }
> h6 { font-size: 0.67em; }
> p  { font-size: 1em; }
> ```

---

## 💡 Example Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Headings and Paragraph Example</title>
</head>
<body>
  <h1>This is H1 Heading</h1>
  <h2>This is H2 Heading</h2>
  <h3>This is H3 Heading</h3>
  <h4>This is H4 Heading</h4>
  <h5>This is H5 Heading</h5>
  <h6>This is H6 Heading</h6>

  <p>This is a paragraph. It contains normal text and represents a block of content in HTML.</p>
</body>
</html>

---


## 💻 HTML Document Example

Below is the full example of the HTML page provided:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chapter-One-Structure</title>
</head>
<body>
    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

    <h1>This is the Main Heading</h1>
    <p>
        This text might be an introduction to the rest of the page. And if the
        page is a long one it might be split up into several sub-headings.
    </p>

    <h2>This is a Sub-Heading</h2>
    <p>
        Many long articles have sub-headings so to help you follow the structure
        of what is being written. There may even be sub-sub-headings (or
        lower-level headings).
    </p>

    <h2>Another Sub-Heading</h2>
    <p>Here you can see another sub-heading.</p>
</body>
</html>
```

---

## 🧠 Explaining Each Tag

### `<!DOCTYPE html>`

**Purpose:**
Tells the browser that this document follows HTML5 standards.

**Note:**
This line should **always appear at the very top** of every HTML page.

---

### `<html>` and `</html>`

**Purpose:**
Defines the beginning and end of an HTML document.

**Example:**

```html
<html lang="en">
  ...content...
</html>
```

**Tip:**
The `lang="en"` attribute specifies that the page language is English.

---

### `<head>` and `</head>`

**Purpose:**
Contains **metadata** about the web page, information that is not displayed on the page itself but helps browsers and search engines understand it.

**Example:**

```html
<head>
  <meta charset="UTF-8">
  <title>My Page Title</title>
</head>
```

---

### `<title>` and `</title>`

**Purpose:**
Defines the **title of the page** that appears in the browser tab.

**Example:**

```html
<title>Chapter-One-Structure</title>
```

**Real-world Use:**
The title helps users identify the page and improves SEO (Search Engine Optimization).

---

### `<meta>` Tags

**Purpose:**
Provide **information about the webpage** such as character encoding and responsive behavior.

**Examples:**

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

* `charset="UTF-8"` ensures the page supports most world languages.
* `viewport` makes the page responsive on mobile and desktop screens.

---

### `<body>` and `</body>`

**Purpose:**
Everything inside these tags appears **on the actual web page** (in the browser window).

**Example:**

```html
<body>
  <h1>Main Content</h1>
  <p>This is visible to users.</p>
</body>
```

---

### `<h1>` and `<h2>` Headings

**Purpose:**
Define headings and subheadings in a document.

* `<h1>` Main heading (used once per page)
* `<h2>` Subheading (used for sections)
* `<h3>` to `<h6>` Lower-level headings for nested structure

**Example:**

```html
<h1>This is the Main Heading</h1>
<h2>This is a Sub-Heading</h2>
```

**Tip:**
Headings help both **readers** and **search engines** understand the structure of your content.

---

### `<p>` Paragraphs

**Purpose:**
Defines a paragraph of text.

**Example:**

```html
<p>This is my first paragraph of text.</p>
```

**Note:**
Always close your paragraph with a `</p>` tag.

---

## ⚙️ Attributes

**Attributes** add extra information to elements.
They appear **inside the opening tag** and are written as `name="value"`.

**Example:**

```html
<p lang="en-us">Paragraph in English</p>
```

* `lang` → Attribute name
* `"en-us"` → Attribute value

**Tip:**
Always write attributes in lowercase and enclose values in quotes.

---

## 🧰 Creating Your First Web Page

**For Windows (Notepad):**

1. Open **Notepad**.
2. Type your HTML code.
3. Save the file as `first-test.html`.
4. Open it in your web browser to see the result.

**For Mac (TextEdit):**

1. Open **TextEdit**.
2. Go to Preferences → Select **Ignore rich text commands in HTML files**.
3. Save as `first-test.html`.
4. Open it with your browser.

---

## 🔍 Viewing Page Source

You can view how any website is built by checking its **source code**.

**Steps:**

1. Open a web page.
2. Right-click → “View Page Source” (or use Ctrl+U).
3. Study the HTML structure.

**Note:**
This is a great way to learn — you can explore how professional developers structure pages.

---

## 🧾 Summary

* HTML pages are **text documents** made of **tags and elements**.
* **Tags** define the **meaning and structure** of content.
* Most tags come in **pairs**: opening and closing.
* **Attributes** give extra information to elements.
* A web page’s structure always includes `<!DOCTYPE>`, `<html>`, `<head>`, and `<body>`.
* Practice writing and viewing your own HTML files to strengthen your understanding.

---

### ✅ Final Example Recap

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Chapter-One-Structure</title>
</head>
<body>
  <h1>This is the Main Heading</h1>
  <p>This text might be an introduction to the rest of the page.</p>
  <h2>This is a Sub-Heading</h2>
  <p>Sub-headings help organize longer content.</p>
</body>
</html>
```

---

💡 **Tip for Students:**
Start by memorizing the basic structure:

```
<!DOCTYPE html>
<html>
  <head>...</head>
  <body>...</body>
</html>
```

Once you master this, building modern web pages becomes much easier! 🚀
