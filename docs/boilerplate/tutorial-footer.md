#Fancy Footers
The footer contains the bottom "rail" or "lip" as well as supporting brand logos and it's own background images.

###Styling The Lip
The lip is configured by the `$body-footer-styles` object, check out the following examples:

**Hiding The Lip Completely**

```js
$body-footer-styles: (
    display:none
);
```

**Simplifying The Lip**

```js
$body-footer-styles:(
    background: white,
    border-radius:0,
    height:12px
);
```

**Automatic Gradient Fill**  
If you specify a `background-color` value and no `background` value, a gradient fill will automatically be generated for you based on the color you specify.

```js
$body-footer-styles:(
    background-color: red
);
```

###Bringing It Home
Here we'll walk through a full customization in detailed steps.

**Step 1**  
Add a bottom margin to the content area and round the bottom corners ever so slightly:

```js
// Content Background
$body-content-styles:(
    background: url("images/acme_content_bg.png"),
    border-radius:0 0 4px 4px,
    margin-bottom:20px
);
```

**Step 2**
Modify the Powered By logo and the nav divider color:

```js
$footer-settings: (
    poweredby-fill: #4D4D4D,
    poweredby-opacity: 100%,
    divider-color: $ui-brand-color
);
```

**Step 4**  
Flood fill the footer background, add some padding to the top and change the text color:

```js
$footer-styles: (
    background: #333,
    padding-top:20px,
    color: #9C9C9C
);
```

**Step 5**
Let's add some branding/logos next to the "Powered By" logo. Download the following images:

| Logo 1:        | Logo 2:        |
| -------------- | -------------- |
| <img src="../tutorial/acme_brand_1.png" width="200"/> | <img src="../tutorial/acme_brand_2.png" width="200"/> |

Now modify your `$footer-settings` to look like this:

```js
$footer-settings: (
    poweredby-fill: #4D4D4D,
    poweredby-opacity: 100%,
    divider-color: $ui-brand-color,
    brand-logos:(
        "images/acme_brand_1.png" 50px 40px,
        "images/acme_brand_2.png" 90px 40px,
    )
);
```

**NOTE: ** The brand logos should always be formatted as `"url" width height,` the comma at the end is required as well.

###Next Steps
You should now have a pretty good idea of what's possible. Check out the [Documentation](docs.md) for all of the possible configuration options, and if you're feeling particularly adventurous check out [Using Custom SCSS](scss.md).
