# User Nav Ideas
The user nav contains a few buttons and menus relevant to the logged in user.

###Un-Buttoning
In this example we'll remove the button styling and tweak things a little to give the user nav a cleaner look.

```sass
$user-nav-button:(
    background:none,
    color:inherit,
    padding-left:10px,
    height:30px
);
```

**Adding Rollovers**  
If you'd like to provide rollover styles, use the following configuration. Note that these are turned off for mobile/touch environments.

```sass
$user-nav-hover-styles:(
    color: red
);
```
