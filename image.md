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
