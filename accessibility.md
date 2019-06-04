# Accessibility

## Buttons

Use tag `<button>` for buttons. Why? Reasons:

- autofocus on `Tab` press
- if you press `Spacebar` key when element is focused it will trigger `click` event
- you can use `disabled` attribute to deactivate button

See [codepen example](https://codepen.io/yesnik/pen/xNMvRK)

## Use ARIA attributes

To make your page visible for screen readers use ARIA attributes (Accessible Rich Internet Applications).

```
<a href="https://facebook.com" aria-label="Facebook"></a>

<button aria-label="Close popup window">X</button>
```
