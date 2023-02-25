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

## Void elements
Not all elements follow the pattern of an opening tag, content, and a closing tag. Some elements consist of a single tag, which is typically used to insert/embed something in the document. 

---

## Attributes 
Attributes contain extra information about the element that won't appear in the content.

An attribute should have:

1. A space between it and the element name.
2. The attribute name, followed by an equal sign.
3. An attribute value, wrapped with opening and closing quote marks.

## Boolean attributes
Boolean attribute is an attribute without values.
Boolean attributes can only have one value, which is generally the same as the attribute name.

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

1. **`<!DOCTYPE html>`:** this used to tell the browser about the version of HTML we use to write a code.
2. **<html>:** this element wraps all the content on the page, it is sometimes known as the root element.
3. **<head>:** this element is a container for everything you want to include on the HTML page such as, keywords, page description, css to style content, character set declaration.
4. **`<meta charset="utf-8">`:** The `meta` is represent the metadata, and the `charset` attribute sets the character set for your document to UTF-8, which includes most characters that used by human languages.
5. **`<title>`:** this sets the title of the page.
6. **`<body>`:** this element contains all the content that displays on the page, including text, images, videos, or whatever else.

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