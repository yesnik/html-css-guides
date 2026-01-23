# CSS Selectors

[Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/Guides/Selectors)

## The next-sibling combinator `+`

It separates two selectors and matches the second element only if it immediately follows the first element, and both are children of the same parent element.

```html
/* Paragraphs that come immediately after any image */
img + p {
  font-weight: bold;
}
```

```html
/* Second li */
li:first-of-type + li {
  color: red;
}
```

## The child combinator `>`

It is placed between two CSS selectors. It matches only those elements matched by the second selector that are the direct children of elements matched by the first.

```html
/* List items that are children of the "my-things" list */
ul.my-things > li {
  margin: 2em;
}
```

## The subsequent-sibling combinator `~`

The subsequent-sibling combinator (~, a tilde) separates two selectors and matches all instances of the second element that follow the first element (not necessarily immediately) and share the same parent element.

In the following example, the subsequent-sibling combinator (~) helps to select and style paragraphs that are both siblings of an image and appear after any image.

```css
p ~ span {
  color: red;
}
```

```html
<article>
  <span>This is not red because it appears before any paragraph.</span>
  <p>Here is a paragraph.</p>
  <code>Here is some code.</code>
  <span>
    This span is red because it appears after the paragraph, even though there
    are other nodes in between.
  </span>
  <p>Whatever it may be, keep smiling.</p>
  <h1>Dream big</h1>
  <span>
    Doesn't matter how many or what kind of nodes are in between, all spans from
    the same parent after a paragraph are red.
  </span>
</article>
<span>
  This span is not red because it doesn't share a parent with a paragraph.
</span>
```

## `:first-child`

The `:first-child` CSS pseudo-class represents the first element among a group of sibling elements.

```css
li:first-child {
  border: 2px solid orange;
}
```

## `:last-child`

The :last-child CSS pseudo-class represents the last element among a group of sibling elements.

```css
li:last-child {
  border: 2px solid orange;
}
```

## `:nth-child()`

The `:nth-child()` CSS pseudo-class matches elements based on the indexes of the elements in the child list of their parents. 
In other words, the `:nth-child()` selector selects child elements according to their position among all the sibling elements within a parent element.

```css
/* Select first 3 elements */
li:nth-child(-n + 3) {
  border: 2px solid orange;
}

/* Select even elements */
li:nth-child(even) {
  background-color: lightyellow;
}

/* Select 5th element */
li:nth-child(5) {
  border: 2px solid orange;
}
```

## `::after`

In CSS, `::after` creates a pseudo-element that is the last child of the selected element. 
It is often used to add cosmetic content to an element with the content property. It is inline by default.

```css
a::after {
  content: " (" attr(href) ")";
}

.broken-link::after {
  content: url("/shared-assets/images/examples/warning.svg");
  display: inline-block;
  width: 12px;
  height: 12px;
}
```

## `::before`

In CSS, `::before` creates a pseudo-element that is the first child of the selected element. 
It is often used to add cosmetic content to an element with the content property. It is inline by default.

```css
a::before {
  content: "🔗";
}

h2::before {
  content: '';
  width: 10px;
  height: 10px;
  background: red;
  display: inline-block;
}
```

## `::first-letter`

The `::first-letter` CSS pseudo-element applies styles to the first letter of the first line of a block container, 
but only when not preceded by other content (such as images or inline tables).

```css
p::first-letter {
  initial-letter: 3;
  font-weight: bold;
  margin-right: 1rem;
  color: brown;
}
```
