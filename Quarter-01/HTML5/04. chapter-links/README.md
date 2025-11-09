# 📘 HTML5 Chapter 4 – Links

## 🗂️ Table of Contents
1. [Introduction to Links](#introduction-to-links)
2. [The `<a>` Anchor Tag](#the-a-anchor-tag)
3. [Creating Basic Links](#creating-basic-links)
4. [Absolute vs Relative URLs](#absolute-vs-relative-urls)
5. [Linking to Other Pages](#linking-to-other-pages)
6. [Opening Links in a New Tab](#opening-links-in-a-new-tab)
7. [Linking Within the Same Page (Anchors)](#linking-within-the-same-page-anchors)
8. [Email Links (`mailto:`)](#email-links-mailto)
9. [Telephone Links (`tel:`)](#telephone-links-tel)
10. [Useful Tips](#useful-tips)
11. [Example: Full HTML Page](#example-full-html-page)
12. [Conclusion](#conclusion)

---

## 🌐 Introduction to Links

Links are one of the **most important elements in HTML**.  
They allow users to **navigate between web pages**, **open files**, **send emails**, or even **call a phone number** — all with a single click.

In HTML, links are created using the **`<a>` tag**, also called the **anchor tag**.

---

## 🔗 The `<a>` Anchor Tag

### 📘 Basic Syntax
```html
<a href="URL">Link Text</a>
```

**Explanation:**
- `<a>` → The anchor element that creates a hyperlink.
- `href` → The **destination address** (URL, file path, or action).
- `Link Text` → The **visible clickable text**.

### ✅ Example
```html
<a href="https://www.google.com">Visit Google</a>
```
**Output:** [Visit Google](https://www.google.com)

---

## 🌍 Creating Basic Links

To create a simple link, use the `href` attribute to point to a destination.

```html
<a href="https://www.wikipedia.org">Go to Wikipedia</a>
```

When clicked, the browser loads the target page.

**💡 Tip:** You can link to **websites**, **files**, or **local HTML pages**.

---

## 🧭 Absolute vs Relative URLs

### 1️⃣ **Absolute URL**
- Contains the **full web address**, including protocol (`https://`).
- Commonly used for **external websites**.

```html
<a href="https://www.devtodeploy.co">Visit DevToDeploy</a>
```

### 2️⃣ **Relative URL**
- Points to another page **within your own website** or project folder.
- No `https://` or full domain is needed.

```html
<a href="about.html">About Us</a>
```

✅ **Best practice:** Use **relative URLs** for internal links and **absolute URLs** for external ones.

---

## 📄 Linking to Other Pages

You can easily link multiple pages in your project:

Example project folder:
```
index.html
about.html
contact.html
```

Link between them:
```html
<a href="contact.html">Contact Us</a>
```

**Note:**  
- Always double-check file paths and names.  
- Use folders for organization (e.g., `/pages/about.html`).

---

## 🪟 Opening Links in a New Tab

To make a link open in a **new browser tab**, use:
```html
target="_blank"
```

Example:
```html
<a href="https://www.youtube.com" target="_blank">Open YouTube</a>
```

✅ **Tip:** Use this when linking to **external websites** to keep your page open.

---

## 🧭 Linking Within the Same Page (Anchors)

You can use links to **jump to different sections of the same page** using IDs.

### Example:
```html
<h2 id="about">About Us</h2>
<a href="#about">Go to About Section</a>
```

When clicked, the link scrolls directly to the `<h2 id="about">` section.

✅ Useful for:  
- Table of contents  
- Long articles  
- FAQ pages

---

## 📧 Email Links (`mailto:`)

You can make a link that opens the user’s email app with a **pre-filled address**.

```html
<a href="mailto:info@devtodeploy.co">Email Us</a>
```

You can also include subject and body:
```html
<a href="mailto:support@devtodeploy.co?subject=Support%20Request&body=Hello!">Email Support</a>
```

📘 **Real-world Use:** Contact links in websites or footers.

---

## ☎️ Telephone Links (`tel:`)

Use `tel:` to make a link that dials a phone number directly (mainly for mobile users).

```html
<a href="tel:+923171291912">Call Now</a>
```

**💡 Tip:** Use international format for better compatibility.

---

## 💡 Useful Tips

- ✅ Use **meaningful link text** (avoid “click here”).
- ✅ Add `title` attributes for tooltips:
  ```html
  <a href="index.html" title="Return to homepage">Home</a>
  ```
- ✅ Use CSS to style links:
  ```css
  a {
      color: blue;
      text-decoration: none;
  }
  a:hover {
      text-decoration: underline;
  }
  ```

---

## 🧾 Example: Full HTML Page

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Links Example</title>
</head>
<body>
    <h1>HTML Links Demonstration</h1>

    <p>Learn more <a href="about.html">About Us</a>.</p>
    <p>Visit <a href="https://www.google.com" target="_blank">Google</a>.</p>
    <p>Jump to the <a href="#contact">Contact Section</a>.</p>

    <h2 id="contact">Contact Us</h2>
    <p>Email: <a href="mailto:support@devtodeploy.co">support@devtodeploy.co</a></p>
    <p>Phone: <a href="tel:+923171291912">+92 317 1291912</a></p>
</body>
</html>
```

---

## 🧠 Conclusion

- Links are essential for **navigation** and **interconnectivity** on the web.  
- The `<a>` tag can link to websites, emails, phone numbers, or even sections on the same page.  
- Understanding links builds the foundation for creating professional, user-friendly websites.

🚀 **Next Step:** Learn how to style and customize links using **CSS pseudo-classes** like `:hover`, `:visited`, and `:active`.
