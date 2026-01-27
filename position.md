# Position elements

`position:`
- `static` (default)
- `relative`
- `absolute` - we can set `position: relative` to a parent block and place the current block within it
- `fixed`
- `sticky`

## Center vertically

```css
.slick-btn {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
}
```

## Button "Scroll up"

We can place a button in the right bottom corner that will be there during scroll:

```css
.btn-up {
  position: fixed;
  right: 30px;
  bottom: 30px;
}
```

## Sticky note

Sticky block will be on the top of the screen when we scroll down a page. When we see an actual position of the block it becomes not sticky.

```html
<p>Lorem ipsum ... (big text here)</p>
<p>Lorem ipsum ... (big text here)</p>
<p>Lorem ipsum ... (big text here)</p>

<div class="positioned">Sticky</div>

<p>Lorem ipsum ... (big text here)</p>
```
```css
.positioned {
  position: sticky;
  top: 10px;
}
```
