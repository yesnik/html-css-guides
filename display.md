# Display

The [display](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/display) CSS property sets whether an element 
is treated as a block or inline box and the layout used for its children, such as flow layout, grid or flex.

```css
display: block;
display: inline-block;
display: none;
display: flex;
display: grid;
```

## Display Grid

A Game: https://cssgridgarden.com/

- `grid-template-rows:`
  - `40px 4em 40px;`
  - `1fr 2fr 1fr;`
- `grid-template-columns:`
  - `60px 200px 60px;` - we have 3 columns
  - `1fr 50px 50px;` - two right columns have fixed width, first column occupies free space
  - `min-content min-content min-content;` - three columns that will have min content width
  - `max-content max-content;` - two columns that will have max content width
  - `1fr 60px;`
  - `1fr 2fr;` 
- `grid-template:` (It's a shorthand property for defining grid columns, grid rows, and grid areas) 
  - `100px 1fr / 50px 1fr;` - here we place grid-template-rows / grid-template-columns values
  - `auto 1fr / auto 1fr auto;`
- `grid-column-start: 1;`
- `grid-column-end:`
  - `4;` - extend the item across multiple columns (start at the 1st vertical grid line and end at the 4th.)
  - `-2` - we can set it to -2 to specify the first grid line from the right.
- `gap: 20px 10px;` - adds gap 20px from top and bottom, 10px from left and right
- `justify-items: right;` - justify items along X
- `align-items: center;` - align items along Y

### 3 columns

```html
<div class="box">
  <div>One</div>
  <div>Two</div>
  <div>Three <br />has <br />extra <br />text</div>
  <div>1</div>
  <div>2</div>
  <div>3 <br />has <br />extra <br />text</div>
</div>

```
```css
.box {
  border: 2px dotted green;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 200px;
  gap: 20px 10px;
}

.box div {
  border: 1px solid red;
}
```

### Change length of the last item

```html
<div class="box">
  <div>One</div>
  <div>Two</div>
  <div>Three <br />has <br />extra <br />text</div>
    <div>1</div>
  <div>Wide item</div>
</div>
```
```css
.box {
  border: 2px dotted green;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 200px;
  gap: 20px 10px;
}

.box div {
  border: 1px solid red;
}

.box div:last-child {
  grid-column: 2 / 4;
}
```
