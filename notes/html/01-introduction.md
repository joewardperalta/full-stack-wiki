# Introduction to HTML

**HTML (HyperText Markup Language)** is the standard language used to build web pages. It provides the structure and meaning of content through elements such as headings, paragraphs, and links. Every website you visit is built using HTML as its foundation.

## What is an HTML?

**HTML** is a markup language used to define the structure and content of a web page. It consists of a set of **tags** that give meaning to different types of content, such as headings, paragraphs, links, and images.

**For example:**

```html
<p>My name is Joeward Peralta</p>
```

This is an example of a **paragraph element (`<p>`)** that contains the text content: "_My name is Joeward Peralta_".

---

## Why is HTML a Markup Language?

**Markup** refers to a system of symbols or tags inserted into a text that describe the _structure_, _meaning_, or _presentation_ of that text. It's not the actual content (the words), but it's the extra information that explains what the content is or how it should be handled.

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

**For example:**

```html
<p>Hello, World</p>
```

- `<p>` is an opening tag that tells the browser to start a paragraph
- `</p>` is a closing tag that tells the browser to end the paragraph
- Anything between `<p>` and `</p>` is treated as a **paragraph content**

They don't show up on the page, but they tell the browser _how to interpret the text_.

---

## Why is HTML a HyperText?

HTML is called a HyperText language because it allows text to contain **links (hyperlinks)** that connect one document to another, letting users jump non-linearly between documents/resources. This ability to interlink documents is what makes the World Wide Web a "web" of connected information.

Unlike printed books (which is read from page 1 to page 100 in sequence), hypertext lets you jump from one document to another via **links**.

**For example:**

```html
<p>
  Learn more about
  <a href="https://developer.mozilla.org/">HTML here</a>.
</p>
```

- Anchor tag `<a>` creates a hyperlink
- Hypertext Reference `href` contains the destination to a page, site, file, or section

The hyper in HTML comes from its ability to embed links inside content. This is what makes the web an interconnected hypertext documents.

---

## What is an HTML Document?

An **HTML document** is a file with a `.html` extension that contains HTML code, which a web browser can read and render into a web page. It includes all the elements and structure needed for a page, such as headings, paragraphs, links, images, and metadata.

The most common HTML file is a `index.html` which is a default HTML page (homepage) of a website or a folder on a server.

When a user visits a domain (e.g., `example.com`) or a subdirectory (e.g., `example.com/blog/`), the web server looks for an **index file** (commonly `index.html`) and serves it automatically.

This convention has existed since the early days of the web and is sill the standard today.

---

### The Basic Structure of an HTML Document

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>This is my first HTML document.</p>
  </body>
</html>
```

- `<!DOCTYPE html>` - tells the browser this is an HTML5 document
- `<html>` - the root element; everything goes inside this
- `<head>` - contains metadata (title, styles, SEO info, etc.)
- `<title>` - defines the page's title (appears on the browser tab)
- `<body>` - contains the visible content (text, images, links, etc.)

### Why use `index.html` instead of any name?

#### 1. Default Behavior of Web Servers

Servers like **Apache**, **Nginx**, **IIS**, and **Node.js** frameworks are usually configured to look for a file named `index.html` when no file is specified in the URL

**For example:**

- `https://example.com/` automatically shows `index.html` in the web browser
- If the homepage is named `home.html`, the visitor must type `https://example.com/home.html` (less user-friendly)

#### 2. User-Friendly URLS

Without `index.html`, users would need to remember file names.

**For example:**

- With `index.html`: `https://myportfolio.com`
- Without `index.html`: `https://myportfolio.com/startpage.html`

Clear URLs make websites easier to access, type, and share.

#### 3. Web Hosting Requirement

Many hosting services like GitHub Pages, Netlify, Vercel, and cPanel require an `index.html` file in the root folder to display the site.

If the uploaded files doesn't contain `index.html`, the server may show a directory listings (all files and folders) or even an error page.

#### 4. Subdirectory Default Pages

`index.html` works not only for the root folder but also for subfolders.

**For example:**

```pgsql
website/
├── index.html        ← main homepage
├── about.html
├── blog/
│    └── index.html   ← blog homepage
└── contact.html
```

Visiting `https://website.com/blog/` automatically shows `blog/index.html`

## Anatomy of an HTML Element

```html
<p>My name is Joeward Peralta</p>
```

This skeleton consists of:

- **Opening tag** - is the `p` tag wrapped in `<>` brackets
- **Content** - is the text in between of the opening tag `<p>` and closing tag `</p>`
- **Closing tag** - is the same as the opening tag but it includes a forward slash `/` before the element name
