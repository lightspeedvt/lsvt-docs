#Styling the Hamburger Menu
The Hamburger Menu has a number of easily configurable customization options as well as full css styling support. Read through and try out the examples below and have fun!


###Colors
The icons and headers will inherit `$ui-brand-color` by default, but you can customize the individual colors using the `$tray-settings` configuration below:

```sass
$tray-settings:(
    color-icon: #9A9A9A,
    color-header: #9a9a9a,
    color-link: #eee
);
```

###Background Image

**Repeating Pattern**
Right click and save the following image into your `output/images/` folder then copy/paste the code below into your settings file and save. You'll notice the `background-size` attribute which scales the texture down from it's original size which is helpful for retina displays.

| Pattern Image: |
| -------------- |
| <img src="../tutorial/acme_tray_bg.jpg" width="200"/> |

```sass
$tray-styles: (
    background: url("images/acme_tray_bg.jpg"),
    background-size: 100px 100px,
    color:#eee
);
```
**Full Image**
Right click and save the following image into your `output/images/` folder then copy/paste the code below into your settings file and save. You'll notice the `background-size` attribute which scales the texture down from it's original size which is helpful for retina displays.

| Background Image: |
| -------------- |
| <img src="../tutorial/acme_tray_full.jpg" width="200"/> |

```sass
$tray-styles: (
    background: url("images/acme_tray_full.jpg"),
    background-size: cover,
    color:#eee
);
```

**Multiple Images**  
It's possible to specify multiple images in the background attribute which we'll explore now. Building off the previous examples we'll now use a repeating pattern with a fixed image in the background. Right click and save the following images into your `output/images/` folder then copy/paste the code below into your settings file and save.

| Pattern Image: | Overlay Image: |
| -------------- | -------------- |
| <img src="../tutorial/acme_tray_bg.jpg" width="200"/> | <img src="../tutorial/acme_tray_stamp.png" width="200"/> |

```sass
$tray-styles: (
    background: (
        url("images/acme_tray_stamp.png"),
        url("images/acme_tray_full.jpg")
    ),
    background-repeat: no-repeat,
    background-position: ( 102% 50%, center ),
    background-size: (180px 150px, cover),
    color:#eee
);
```
