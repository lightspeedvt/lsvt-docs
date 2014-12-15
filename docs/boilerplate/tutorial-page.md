#Better Backgrounds
Using page overlays and multiple backgrounds is a great way to add visual interest and spice up your custom themes. The following examples provide some ideas and inspiration.

***

###Adding an overlay
Building off our previous work, we'll download a tranparent image and add it as an overlay:

| Overlay Image: |
| -------------- |
| <img src="../tutorial/acme_overlay.png" width="200"/> |

Using the `$page-overlay-styles` config we'll do a number of things:

1. Add two instances of our "Boilerplate" mascot by specifying multiple background images.
2. Set the width of our overlay to `1200px` and center it on the page using a combination of `left:50%` and setting it's `margin-left` to half of it's width `-600px`
3. Use `background-size` to scale down the images 

```sass
$page-overlay-styles:(
    background: (
        url( "images/acme_overlay.png") top left no-repeat,
        url( "images/acme_overlay.png") top right no-repeat,
    ),
    width:1200px,
    left:50%,
    top:160px,
    margin-left:-600px,
    background-size: 180px 360px
);
```
