# Assets directory

The assets directory contains your un-compiled assets such as Stylus or Sass files, images, or fonts.

📦assets
 ┣ 📂images
 ┣ 📂scss
 ┣ 📂svg

## Images
Inside your templates, if you need to link to your assets directory use 

```bash
~/assets/your_image.png
``` 
with a slash before assets.


## Styles
React lets you define the CSS files/modules/libraries you want to set globally (included in every page). In the index.js you can easily add your styles using the CSS Property.
![Import CSS](/assets/images/css.png)

Some CSS files are defined in the source code.

![CSS Structural](/assets/images/css-structural.png)

## Sass & Sass Loader
Install Sass and Sass Loader to render the CSS file.
Configure Scss inside the craco.config.js file.

![Sass Loader](/assets/images/sass.png)

## Fonts
You can import a font-like link via public/index.html or import a @font-face link in the assets folder.

```bash
  <link
      href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap"
      rel="stylesheet"
  />
```

Example for @font-face:

![Font Structural](/assets/images/font-structural.png)

in ***font.face.css***

![Fonts](/assets/images/font-face.png)