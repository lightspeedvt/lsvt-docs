#Cookie Crumbs
The "cookie crumb" navigation gives the user a sense of where they are in the system and allows for quick access to previously viewed pages.

###Simplifying Things
Let's simplify the crumb menu's appearance and change the color of the dividers:

```sass
$crumb-menu-styles:(
    background: white,
    box-shadow:none,
    border-radius:0
);

$crumb-menu-settings:(
    divider-color: $ui-brand-color
);
```

