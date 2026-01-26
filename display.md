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
