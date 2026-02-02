# Image

## Place an image in a rectangle

```html
<div class="product-thumb">
  <img src="images/car.jpg" alt="">
</div>
<h3 class="product-name">BMW</h3>
```
```css
.product-thumb {
  width: 100%;
  height: 430px;
  position: relative;
  overflow: hidden;
}

.product-thumb img {
  width: 100%;
  height: 100%;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  object-fit: cover; /* Allows to save image's proportions */
}
```

## Image in a CSS

### Logo

```html
<a href="#" class="footer-logo">&nbsp;</a>
```
```css
.footer-logo {
  display: block;
  width: 63px;
  height: 56px;
  background-image: url(../images/logo-light.svg);
  background-repeat: no-repeat;
  background-size: contain;
}
```

### Close button at modal

```html
<div class="modal" id="modal">
  <nav class="nav">
    <a href="#" class="nav-link">Main</a>
    <a href="#" class="nav-link">Menu</a>
    <a href="#" class="nav-link">Contacts</a>
  </nav>
  <button class="modal-close"></button>
</div>
```
```css
.modal-close {
  display: block;
  width: 22px;
  height: 22px;
  background-image: url(../images/close.svg);
  background-repeat: no-repeat;
  background-size: contain;
  background-color: transparent;
  border: none;
  position: absolute;
  top: 20px;
  right: 20px;
}
```
