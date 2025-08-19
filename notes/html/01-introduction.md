# Introduction to HTML

## What is an HTML?

**HTML (HyperText Markup Language)** is a markup language used to define the structure and content of a web page. It consists of a set of **tags (elements)** that give meaning to different types of content, such as headings, paragraphs, links, and images.

### For example

```html
<p>My name is Joeward Peralta</p>
```

This is an example of a **paragraph element** (`<p>`) that contains the text content: "_My name is Joeward Peralta_".

## Why is HTML a Markup Language?

**Markup** refers to a system of symbols or tags inserted into a text that describe the _structure_, _meaning_, or _presentation_ of that text. It's not the actual content (the words), but it's the **extra information** that explains what the content is or how it should be handled.

- **System** is a set of rules everyone follows
- **Symbols/Tags** are special characters or keywords that surround or annotate text, giving it structure or meaning

### Rules

HTML is a markup system that contains **rules (syntax)**:

- Tags must be inside angle brackets `< >`
- Must have an opening and closing tags `<p>...</p>` except for tags that are self-closing such as an image tag `<img>`
- Every page must start with an HTML tag `<html>...</html>`
- Headings use `<h1>` to `<h6>`
- Links use `<a href="">`
- Content goes inside `<body>`

### For example

```html
<p>Hello, World</p>
```

- `<p>` is an opening tag that tells the browser to start a paragraph
- `</p>` is a closing tag that tells the browser to end the paragraph
- Anything between `<p>` and `</p>` is treated as a **paragraph content**

They don't show up on the page, but they tell the browser _how to interpret the text_.

## Why is HTML a HyperText?

HTML is called a HyperText language because it allows text to contain **links (hyperlinks)** that connect one document to another, letting users jump non-linearly between documents/resources. This ability to interlink documents is what makes the World Wide Web a "web" of connected information.

Unlike printed books (which is read from page 1 to page 100 in sequence), hypertext lets you jump from one document to another via **links**.

### For example

The hyper in HTML comes from its ability to embed links inside content.

```html
<p>
  Learn more about
  <a href="https://developer.mozilla.org/">HTML here</a>.
</p>
```

- Ancor tag `<a>` creates a hyperlink
- Hypertext Reference `href` contains the destination to a page, site, file, or section

This is what makes the web an interconnected hypertext documents.
