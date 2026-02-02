# Box Shadow

## Add a border inside a button

```html
<button class="btn btn--outline">
    Submit
</button>
```
```css
.btn {
    border: none;
    background-color: transparent;
    outline: none;
    padding: 10px 15px;
}
.btn--outline:hover,
.btn--outline:active {
    box-shadow: inset 0 0 0 3px white;
}
```
