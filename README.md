## Using React Portal to render a modal

This solves the problem of a modal not covering up all underlying content. It uses the concept of portals from ReactDom to keep parent-child click events while rendering one item over another.

### Notes

* Our component (the modal) doesn't return straight JSX, but rather `ReactDom.createPortal(JSX, document.getElementById('portal'))`
* The 'portal' id in the document is declared in `/public/index.html` outside the root element.

### Source

Based on the [video](https://www.youtube.com/watch?v=LyLa7dU5tp8) by Kyle at Web Dev Simplified.
