#Tweaking the logo
Changing the logo's position is now built in to the theming process and provides an easy way to make your theme stand out, especially when combined with customizations to the navigation menu.

###Logo Position
There are three positioning options for the logo: `default`, `center`, and `inline` check out the details for each below.

**Default Position**  
The `default` position will place the logo the top-left of the header with the navigation below. You don't have to specify this type of positioning in your configuration as it is the *ahem* default.

**Center Position**  
The `center` position will center the logo in the header with the navigation positioned below. Add the following property to your previously defined `$header-settings` object:

```js
logo-position: center
```

**Inline Position**  
The `inline` position will place logo in the top-left of the header with the navigation positioned beside it on the right. Add the following property to your previously defined `$header-settings` object:

```js
logo-position: inline
```

###Logo Offset
If you've implemented the `inline` position above you'll notice that things are a bit jumbled up now. Add the following property to the `header-settings` object in order to push the logo and navigation down and add some spacing to the right side.

```js
logo-offset:(
    top:50px,
    right:20px
)
```

**Additional Info:** You can use `logo-offset` for all logo positions and can specify `top`, `left`, `right` and `bottom` properties.

###Nav Offset
We're looking good but that pesky nav is not quite right. You can adjust it's position via the `$nav-settings` object like so:

```js
// Nav
$nav-settings: (
    offset:(
        top:10px
    )
);
```
