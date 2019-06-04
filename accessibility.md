# Accessibility

## Buttons

Use tag `<button>` for buttons. Why? Reasons:

- autofocus on `Tab` press
- if you press `Spacebar` key when element is focused it will trigger `click` event
- you can use `disabled` attribute to deactivate button

See [codepen example](https://codepen.io/yesnik/pen/xNMvRK)

## Labels

Use `<label>` tag for form inputs:

```html
<label>
  Car
  <input type="text" name="car">
</label>

<label for="speed">Speed</label>
<input id="speed" type="range" name="speed">
```

If you don't need label according to design, hide it visually. But don't use `display: none`, 
because it'll hide label from screen readers.

## Use link as fallback

If you have a login page on your site and want to use login popup, use link on button that opens popup. It'll allow users to login via login page if javascript is disabled in their browser.

```html
<a href="/login" class="button">Login</a>
```

## Use ARIA attributes

To make your page visible for screen readers use ARIA attributes (Accessible Rich Internet Applications).

```html
<a href="https://facebook.com" aria-label="Facebook"></a>

<button aria-label="Close popup window">X</button>
```
