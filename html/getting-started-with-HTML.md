# Getting started with HTML

---

## What is HTML ?
HTML (HyperText Markup Language) is a markup language that tells web browsers how to structure the web pages you visit.

---

## Elements in HTML 
HTML consists of a series of elements, which you use to enclose, wrap, or mark up different parts of content to make it appear or act in a certain way

---

## Anatomy of an HTML element 
1. **The opening tag:** This opening tag marks where the element begins or starts to take effect. 
3. **The content:** This is the content of the element.
4. **The closing tag:** This marks where the element ends.

> The element is the opening tag, followed by content, followed by the closing tag.

---

## Nesting elements 
Elements can be placed within other elements. This is called nesting.

```
<p>
  My cat is <strong>very</strong> grumpy.
</p>
```

---

## Block versus Inline elements

**Block**
1. A block-level element appears on a new line
2. A block-level elements are usually represent structural elements on the page such as, headings, paragraphs, lists, navigation menus, or footers
3. A block-level element can't be nested inside an inline element, but it can be nested inside another block-level element.

**Inline**
1. Inline elements are contained within block-level elements
2. An inline element will not appear in a new line
3. It typically used with text

---

## Void element
is consist of a single tag, which is typically used to insert/embed something in the document. 

---

## Attributes 
Attributes contain extra information about the element that won't appear in the content.

An attribute should have:

1. A space between it and the element name.
2. The attribute name, followed by an equal sign.
3. An attribute value, wrapped with opening and closing quote marks.

## Boolean attributes
Boolean attribute is an attribute without values. it can only have one value, which is generally the same as the attribute name.

`<input type="text" disabled="disabled" />`, This is the full one

`<input type="text" disabled />`, This is the boolean one

---

## Anatomy of an HTML document

```
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <title>My test page</title>
  </head>
  <body>
    <p>This is my page</p>
  </body>
</html>
```

**`<!DOCTYPE html>`:** *this tell the browser about the version of HTML we use to write a code*.
1. **Quirks mode**:  this mode is exists to support the websites that came before W3 standards
2. **Full standards mode:** this mode is used the HTML and CSS specification to render your webpage well
3. **Almost standards mode:** this mode is the same as `full standard mode` but it has a small numbers of quirks

**`<html>`:** this element wraps all the content on the page, it is sometimes known as the root element.

**`lang="en"`**, this attribute specify the main language of the webpage

**`<head>`:** this element is a container for everything you want to include on the HTML page such as, keywords, page description, linking resources, character set declaration.

**`<title>`:** this sets the title of the page.

**`<body>`:** this element contains all the content that displays on the page, including text, images, videos, or whatever else.

---

## Meta

The meta represent the metadata

**charset="UTF-8":** this attribute sets the characters set of your document to `UTF-8`, which includes most characters that used by human languages

`<meta charset="UTF-8" />`

**description:** this adds a description of your webpage

`<meta name="description" content="this is the purpos of my website" />`

**author:** this adds an autor of the website

`<meta name="author" content="kevin jonson" />`

**viewport:** this used to setting a viewport to your website to make it looks good in all devices 

`<meta name="viewport" content="width=device-width, initial-scale=1.0">`

---

## Linking Resources

it used to link external stylesheets and scripts files to the document

`<link href="style.css" rel="stylesheet" />`, this links our stylesheet file

`<script src="app.js">`, this links our script file

---

## White spaces in HTML
No matter how much whitespace you use inside HTML element content, the HTML parser reduces each sequence of whitespace to a single space when rendering the code. So why use so much whitespace? **The answer is readability**.

---

## Entity
in HTML, we use it when we needs to include a special character in text

| Literal character | Character reference equivalent |
| :---------------- | :----------------------------- |
| `<`               | `&lt;`                         |
| `>`               | `&gt;`                         |
| `"`               | `&quot;`                       |
| `'`               | `&apos;`                       |
| `&`               | `&amp;`                        |

`<p>In HTML, you define a paragraph using the &lt;p&gt; element.</p>`

---

## HTML Comments
we use comments to write a notes, leave explain for our code