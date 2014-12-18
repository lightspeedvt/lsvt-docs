#Customizing Your Theme
This is where the fun begins, we'll walk through prepping your newly created theme/branch and also perform some basic customizations in order to get you familiar with the process.


***

###Prep Work
1. Open the file `scss/_theme.scss` which is located in your project folder.
2. Delete the image files located in `/output/images`

***

###FYI - Settings vs. Styles
Most of the configuration objects have an identifier that relates to how they are compiled or used in the framework. Any properties defined as part of a `-styles` object will be added as CSS which allows you to use any styles you'd like. Properties defined in a `-settings` object are typically used to configure children of elements or non-css properties.

**NOTE: ** You don't have to copy/paste these, they are for example only.

**Example `-styles` object:**  
```sass
$header-styles: (
    height: 120px,
    margin-bottom: 10px,
    // Any CSS other properties
);
```

**Example `-settings` object:**  
```sass
$header-settings: (
    logo-position: center
    // Non-CSS settings
);
```

***

###Adding Images
Right-click on each of these images and save them to the folder `/output/images/`  

| Logo:         | Footer:       |
| ------------- | ------------- |
| <img src="../tutorial/acme_logo_red.png" width="200"/> | <img src="../tutorial/acme_footer_shadow.png" width="400"/> |

| Page Background: | Content Background: |
| ---------------- | ------------------- |
| <img src="../tutorial/acme_page_bg.jpg" style="width:300px;height:150px !important;"/> | <img src="../tutorial/acme_content_bg.png" style="width:300px;height:150px !important;"/> |

***

###Setting Custom Values
Once you've downloaded the images, make sure you have Grunt running and let's get to work! As you proceed down this page, read the descriptions and then copy/paste the code into your `_theme.scss` file. Save the file each time you paste in new code and watch the changes happen in real time.
***

**Logo**  
Specify both the url of the logo as well as `width` and `height` values. Note that these should **NOT** be the actual dimensions of the image, but rather the **display size**. In this case, the logo image is quite large but is scaled down to remain sharp on "retina" aka "hi-dpi" displays.

```sass
// Logo Settings
$header-settings: (
    logo-url: "images/acme_logo_red.png",
    logo-width: 178px,
    logo-height: 61px
);
```

***

**Accent Color**  
Color the icons and the "rail" above the page when the Hamburger Menu is opened:

```sass
// Accent Color
$ui-brand-color: #c1011a;
```

***

**Hamburger Menu**  
Set the `background` to a gradient:

```sass
// Hamburger Menu
$tray-styles:(
    background: linear-gradient(to bottom, rgb(45, 45, 45), rgb(81, 81, 81)),
    color:#eee
);
```

***

**Page Background**  
Specify the image you've downloaded along with some properties for positioning, etc:

```sass
// Page Background
$page-styles:(
    background: url( "images/acme_page_bg.jpg" ) top center no-repeat,
    background-color: #dbdbdb
);
```

***

**Content Background**  
Specify the image you've downloaded along with some properties for positioning, etc:

```sass
// Content Background
$body-content-styles:(
    background: url("images/acme_content_bg.png")
);
```

***

**Footer**  
Set a background image and push the footer down using `padding-top`:

```sass
// Footer Settings
$footer-styles:(
    background: url( "images/acme_footer_shadow.png") center -120px no-repeat,
    padding-top: 30px
);
```

***

###Congratulations!
You've just built your first theme and and it's looking pretty good. Now that the hard stuff is out of the way, we'll now cover some techniques that will help take your theming skills to the next level!

***

- [Styling the Hamburger Menu](tutorial-hamburger.md)
- [Better Backgrounds](tutorial-page.md)
- [Tweaking The Logo](tutorial-logo.md)
- [Navbars & Buttons](tutorial-nav.md)
- [User Nav Ideas](tutorial-user.md)
- [Cookie Crumbs](tutorial-crumbs.md)
- [Fancy Footers](tutorial-footer.md)

