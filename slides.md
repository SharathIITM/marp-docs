---
marp: true
title: Product Documentation Presentation
author: Sharath
paginate: true
theme: default
---

<!-- Custom Theme -->
<style>
section {
  font-family: "Segoe UI", sans-serif;
  padding: 32px;
}

h1, h2, h3 {
  color: #004aad;
}

footer {
  font-size: 12px;
  color: #777;
}

.code-box {
  background: #f4f4f4;
  padding: 10px;
  border-radius: 8px;
  font-size: 14px;
}

.bg-dark {
  background-color: #0b0f19;
  color: #ffffff;
}
</style>

<!-- _class: lead -->

# Product Documentation Overview  
### Using Marp for Version-Controlled Presentations

**Email:** 22f2001638@ds.study.iitm.ac.in

---

# Why Marp?

- Markdown-driven presentations  
- Easily version-controlled (GitHub, GitLab)
- Export to:
  - PDF  
  - HTML  
  - PPTX  
  - PNG/JPEG
- Developer-friendly (code blocks, diagrams, math)
- Ideal for product documentation

---

<!-- _class: bg-dark -->

# Custom Theme (Inside Markdown)

Marp allows custom theming directly inside your `.md` file:

```css
section {
  background: #0b0f19;
  color: white;
}
```

This keeps documentation portable and Git-friendly.

---

# Background Image Demo

![bg cover](images/background.jpg)

## Slide with a Background Image

This slide uses:

```
![bg cover](images/background.jpg)
```

Make sure the image exists under `images/background.jpg`.

---

# Algorithm Complexity Example

Marp supports math using **KaTeX**.

### Big-O Notation

Inline:  
`Time = O(n \log n)`

Block:

$$
T(n) = n \log n + 3n + 2
$$

### Recurrence Example

$$
T(n) = 2T\left(\frac{n}{2}\right) + n
$$

By Master Theorem:

$$
T(n) = O(n \log n)
$$

---

# Code Example (Python API Snippet)

```python
def get_user(id):
    return database.fetch("SELECT * FROM users WHERE id = ?", id)
```

```bash
marp slides.md --pdf --allow-local-files
```

---

# Custom Slide Styling (Directives)

<!-- _color: #ff5733 -->
<!-- _header: **API Documentation** -->
<!-- _footer: *Product Docs* -->

## Highlighted Slide

You can style individual slides using Marp directives:

```
<!-- _color: red -->
<!-- _backgroundColor: #111 -->
<!-- _header: Title -->
```

---

# Folder Structure (Recommended)

```
project-docs/
├── slides.md
├── images/
│   └── background.jpg
├── themes/
│   └── custom.css
└── package.json
```

---

# Exporting the Presentation

### HTML

```
marp slides.md -o slides.html
```

### PDF

```
marp slides.md --pdf --allow-local-files
```

### PowerPoint

```
marp slides.md --pptx
```

---

# End

Thank you!

For documentation updates:  
**Email:** 22f2001638@ds.study.iitm.ac.in
