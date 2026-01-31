## 1️⃣ Semantic layout tags (VERY important for jobs)

These replaced the old “div soup” and are **non-negotiable** in modern HTML.

**Must-know semantic tags:**

* `<header>` – top section of a page or section
* `<nav>` – navigation links
* `<main>` – main content (only ONE per page)
* `<section>` – grouped content with a theme
* `<article>` – standalone content (blog post, card, comment)
* `<aside>` – sidebar / related content
* `<footer>` – bottom info (copyright, links)

### Why employers care

* Accessibility (screen readers)
* SEO
* Clean, readable code
* Better Lighthouse scores

### Example layout

```html
<header>
  <nav>...</nav>
</header>

<main>
  <section>
    <article>...</article>
  </section>
  <aside>...</aside>
</main>

<footer>...</footer>
```

### Quick check 🧠

👉 When would you choose `<article>` instead of `<section>`?

---

## 2️⃣ Text & content tags (not just `<div>` and `<span>`)

**Headings (SEO + accessibility):**

* `<h1>` → `<h6>` (hierarchy matters!)

**Text semantics (often misused):**

* `<p>` – paragraph
* `<strong>` – important (not just bold)
* `<em>` – emphasis (not just italic)
* `<mark>` – highlighted text
* `<code>` – inline code
* `<pre>` – preformatted text

❌ Avoid:

```html
<b>Important</b>
<i>Emphasis</i>
```

✅ Prefer:

```html
<strong>Important</strong>
<em>Emphasis</em>
```

### Quick check 🧠

👉 Why is using `<strong>` better than `<b>` in professional code?

---

## 3️⃣ Links, media & assets (daily use)

**Essential tags:**

* `<a>` – links
* `<img>` – images
* `<video>` / `<audio>` – media
* `<source>` – responsive media

**Job-critical detail:**
Always use `alt` on images:

```html
<img src="logo.png" alt="Company logo" />
```

### Pro tip employers love

```html
<a href="/docs" target="_blank" rel="noopener noreferrer">
```

### Quick check 🧠

👉 What problem does `alt` text solve?

---

## 4️⃣ Forms (this is where many devs fail interviews)

**Core form tags:**

* `<form>`
* `<label>` (accessibility!)
* `<input>`
* `<textarea>`
* `<select>` / `<option>`
* `<button>`

Example:

```html
<label for="email">Email</label>
<input id="email" type="email" required />
```

### Interview-level details:

* `type="email"`, `password`, `number`
* `required`, `disabled`, `readonly`
* `name` attribute (important for backend!)

### Quick check 🧠

👉 Why is `<label>` important beyond just UX?

---

## 5️⃣ Tables (still relevant)

* `<table>`
* `<thead>`, `<tbody>`
* `<tr>`, `<th>`, `<td>`

Used for **data**, not layout.

---

## 6️⃣ Meta & head tags (often forgotten, very job-relevant)

Inside `<head>`:

* `<meta charset="UTF-8">`
* `<meta name="viewport">`
* `<meta name="description">`
* `<link rel="stylesheet">`
* `<script defer>`

### Pro tip

```html
<script src="app.js" defer></script>
```

👉 avoids blocking page rendering

---

## 7️⃣ Universal attributes (apply to MANY tags)

Must know:

* `class`
* `id`
* `data-*`
* `hidden`
* `aria-*` (accessibility!)

Example:

```html
<button data-id="123" aria-label="Close modal">
```

---

## Mini recap 🔁

If you remember only **5 things**, remember these:

1. Use **semantic tags**, not div soup
2. Heading hierarchy matters
3. `alt`, `label`, and `aria-*` are NOT optional
4. Forms need real structure
5. HTML ≠ styling (that’s CSS’s job)

