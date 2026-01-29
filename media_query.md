# Media Query

The CSS Media Query gives you a way to apply CSS only when the browser and device environment matches a rule that you specify, for example "viewport is wider than 480 pixels". 
Media queries are a key part of responsive web design, as they allow you to create different layouts depending on the size of the viewport.

- See [Mobile Screen Resolution Stats Worldwide](https://gs.statcounter.com/screen-resolution-stats/mobile/)
- See [Bootstrap Breakpoints](https://getbootstrap.com/docs/5.3/layout/breakpoints/)

Broadly, you can take two approaches to responsive design:

1. **Desktop first**. You can start with your desktop or widest view and then add breakpoints to move things around as the viewport becomes smaller.
  ```css
  @media (min-width: 360px) {
    /* ... */
  }
  @media (min-width: 768px) {
    /* ... */
  }
  ```
2. **Mobile first**. You can start with the smallest view and add layout as the viewport becomes larger. It is quite often the best approach to follow.
  ```css
  @media (max-width: 1199px) {
    /* ... */
  }
  @media (max-width: 991px) {
    /* ... */
  }
  ```

The view for the very smallest devices is quite often a simple single column of content, much as it appears in normal flow. 
This means that you probably don't need to do a lot of layout for small devices — order your source well and you will have a readable layout by default.
