# HTML5 tags

## `<blockquote>` and `<cite>`

The `<blockquote>` HTML element indicates that the enclosed text is an extended quotation. 
Usually, this is rendered visually by indentation. A URL for the source of the quotation may be given using the `cite` attribute,
while a text representation of the source can be given using the `<cite>` element.

```html
<blockquote>
    Action may not always bring happiness, but there is no happiness without action.
</blockquote>
<cite>Benjamin Disraeli</cite>
```
```html
<div>
  <blockquote cite="https://www.huxley.net/bnw/four.html">
    <p>
      Words can be like X-rays, if you use them properly—they’ll go through
      anything. You read and you’re pierced.
    </p>
  </blockquote>
  <p>—Aldous Huxley, <cite>Brave New World</cite></p>
</div>
```

## `<header>`

The `<header>` HTML element represents introductory content, typically a group of introductory or navigational aids. 
It may contain some heading elements but also a logo, a search form, an author name, and other elements.

```html
<header>
  <a class="logo" href="#">Cute Puppies Express!</a>
</header>

<article>
  <header>
    <h1>Beagles</h1>
    <time>08.12.2014</time>
  </header>
  <p>
    I love beagles <em>so</em> much! Like, really, a lot. They’re adorable and
    their ears are so, so snugly soft!
  </p>
</article>
```

## `<footer>`

The `<footer>` HTML element represents a footer for its nearest ancestor sectioning content or sectioning root element.
A `<footer>` typically contains information about the author of the section, copyright data or links to related documents.

```html
<article>
  <h1>How to be a wizard</h1>
  <ol>
    <li>Grow a long, majestic beard.</li>
    <li>Wear a tall, pointed hat.</li>
    <li>Have I mentioned the beard?</li>
  </ol>
  <footer>
    <p>© 2018 Gandalf</p>
  </footer>
</article>
```

## `<nav>`

The `<nav>` HTML element represents a section of a page whose purpose is to provide navigation links,
either within the current document or to other documents. Common examples of navigation sections are menus, tables of contents, and indexes.

```html
<nav class="crumbs">
  <ol>
    <li class="crumb"><a href="#">Bikes</a></li>
    <li class="crumb"><a href="#">BMX</a></li>
    <li class="crumb">Jump Bike 3000</li>
  </ol>
</nav>
```

## `<main>`

Holds content that is directly related to or expands upon the central topic of the page. 
Moreover, it helps screen readers and other assistive technologies understand where the main page content begins.

```html
<main>
  <p>
    Geckos are a group of usually small, usually nocturnal lizards. They are
    found on every continent except Antarctica.
  </p>

  <p>
    Many species of gecko have adhesive toe pads which enable them to climb
    walls and even windows.
  </p>
</main>
```

## `<section>`

It demarcates a thematic grouping of content. Each section typically includes a heading element 
and associated content within `<div>` and `<p>`. E.g.: introduction, blog entries, contact information.

```html
<h1>Choosing an Apple</h1>
<section>
  <h2>Introduction</h2>
  <p>
    This document provides a guide to help with the important task of choosing
    the correct Apple.
  </p>
</section>
```

## `<article>`

A self-contained composition in a document that is independently distributable or reusable. 
E.g. a forum post, a magazine article, blog entry.

## `<aside>`

Holds content related to the content surrounding it. E.g.: related reading links, glossaries.

## `<address>`

The `<address>` HTML element indicates that the enclosed HTML provides contact information for a person or people, or for an organization.

```html
<address>
  <a href="mailto:kenny@example.com">kenny@example.com</a><br />
  <a href="tel:+54150001234">+5 (415) 000‑1234</a>
</address>
```

## `<mark>`

The `<mark>` HTML element represents text which is marked or highlighted for reference or notation purposes due to the marked passage's relevance in the enclosing context.

```html
<p>
  Several species of <mark>salamander</mark> inhabit the temperate rainforest of
  the Pacific Northwest.
</p>
```

## `<figure>` and  `<figcaption>`

Used in conjunction with the `<figcaption>` element to mark up diagrams, illustrations, photos, and code listings, etc.

```html
<figure>
  <img
    src="/shared-assets/images/examples/elephant.jpg"
    alt="Elephant at sunset" />
  <figcaption>An elephant at sunset</figcaption>
</figure>
```

## `<q>`

```html
<p>
    Oprah Winfrey said: 
    <q>You define your own life. Don’t let other people write your script.</q>
</p>
```


