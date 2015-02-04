#Overview
This page lists all of the settings available for the Boilerplate. All of the values shown are the defaults which you can override.

***

###Globals

```sass
$link--color: inherit;
$ui-border: 0 0 0 1px rgba(0,0,0,0.2);
$ui-brand-color: #3492cf;

$button-styles:(
    background-color: lightgray,
    color: inherit,
    text-shadow: 0 1px white,
    padding: 0 .6em,
    border-radius: 2px,
    box-shadow: (0 0 0 1px rgba(255,255,255,0.2) inset, 0 0 0 1px rgba(0,0,0,0.1)),
    font-weight: bold,
    height: 1.8em
);

$debug: false;
```

**NOTE: ** If you set `$debug: true` in your `_theme.scss` you will see borders and backgrounds on each element which can help diagnose issues.

###Hamburger Menu

```sass
$tray-styles:(
    background: url("images/bg-tray.jpg"),
    background-size: 300px 300px
);

$tray-settings:(
    height-admin: 250px,
    height-normal: 190px,
    color-icon: $ui-brand-color,
    color-header: $ui-brand-color,
    color-link: #999,
    color-rail: $ui-brand-color
);

$tray-overlay-styles: (
    // No defaults
);
```

###Page

```sass
$page-styles: (
    background: url( "images/bg-site.jpg" ) top center no-repeat,
    background-color: #dbdbdb
);

$page-overlay-styles: (
    position:absolute,
    top:0, left:0, right:0, bottom: 0
);
```

###Custom Page Settings

```sass
$main-menu-styles:();

$training-center-styles:();
```

###Header

```sass
$header-styles: (
    height: 120px,
    margin-bottom: 10px
);

$header-settings: (
    logo-url: "images/logo.png",
    logo-width: 270px,
    logo-height: 50px,
    logo-position: default,
    logo-offset:(
        top: 20px,
        left: -14px,
        bottom: 10px,
        right: 0
    )
);

$location-name-styles: (
    font-weight:500,
    margin-top:1em,
    color: inherit
);
```

###Navigation

```sass
$nav-styles: (
    background:none,
    padding: 0,
);

$nav-settings: (
    offset:(
        top: 0,
        left: 0,
        bottom: 0,
        right: 0
    ),
    navbar-image: none,
    navbar-cap-width: 0

);

$nav-button-styles:(
    // Inherits all properties of $button-styles
    margin-right: 4px
);

$nav-hover-styles:(
    // No defaults
);

$nav-divider-styles: (
    width: 1px,
    top:0,
    bottom:0
);

$search-input-styles: (
    background:white,
    color:inherit,
    text-shadow:none,
    font-weight:normal,
    border-radius: $radius 0 0 $radius // Uses the radius from $nav-button-styles by default
);

$search-button-styles: (
    // Inherits all properties of $nav-button-styles
);

```

###User Navigation/Menu

```sass
$user-nav-button: (
    border-radius: 0 0 2px 2px
);

$user-nav-hover-styles:(
    // No defaults
);

$user-nav-styles: (
    font-size: map-get( $font, size-small )
);
```

###Crumb Navigation

```sass
$crumb-nav-styles: (
    // No defaults
);

$crumb-menu-styles: (
    background-color: #eee,
    padding:6px 8px,
    box-shadow: ($ui-border inset, 0 3px 3px rgba(0,0,0,0.2)),
    border-radius: 4px 4px 0 0,
    text-shadow: 0 1px #eee,
    font-size: map-get( $font, size-boilerplate ),
    min-height:28px
);

$crumb-menu-settings: (
    divider-color: rgba(0,0,0,0.3)
);

```

###Body (Content Area)

```sass
$body-styles: (
    // No defaults
); 

$body-content-styles: (
    background: url("images/bg-body.png"),
    background-size: 100% auto,
    position:relative,
    padding-top: 2em,
    padding-bottom: 2em,
    margin-bottom: 10px
);

$body-footer-styles: (
    background-color: #eee,
    height: 14px,
    box-shadow: $ui-border inset,
    border-radius: 0 0 4px 4px
);
```

###Footer

```sass
// Footer
$footer-styles: (
    height: auto,
    background: none,
    padding-bottom:40px
);

$footer-settings: (
    poweredby-fill: gray,
    poweredby-opacity: 80%,
    divider-color: rgba(0,0,0,0.2),
    brand-logos:()
);
```
