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

📦scss
 ┣ 📂variables
 ┃ ┣ 📜_variables-components.scss
 ┃ ┗ 📜_variables.scss
 ┣ 📜app-loader.scss
 ┣ 📜custom-antd.scss
 ┣ 📜style-rtl.scss
 ┣ 📜style.scss
 ┗ 📜theme.scss

 ## Sass & Sass Loader
 Install Sass and Sass Loader to render the CSS file.
 Configure Scss inside the craco.config.js file.

 ![Sass Loader](/assets/images/sass.png)

## Fonts
You can import a font-like link via public/index.html or import a @font-face link in the assets folder.

![Fonts](/assets/images/fonts.png)

Example for @font-face:

📦fonts
 ┣ 📜iCielGothamRounded-Bold.eot
 ┣ 📜iCielGothamRounded-Bold.svg
 ┣ 📜iCielGothamRounded-Bold.ttf
 ┣ 📜iCielGothamRounded-Bold.woff
 ┣ 📜iCielGothamRounded-Bold.woff2
 ┣ 📜iCielGothamRounded-BoldItalic.eot
 ┣ 📜iCielGothamRounded-BoldItalic.svg
 ┣ 📜iCielGothamRounded-BoldItalic.ttf
 ┣ 📜iCielGothamRounded-BoldItalic.woff
 ┣ 📜iCielGothamRounded-BoldItalic.woff2
 ┣ 📜iCielGothamRounded-Book.eot
 ┣ 📜iCielGothamRounded-Book.svg
 ┣ 📜iCielGothamRounded-Book.ttf
 ┣ 📜iCielGothamRounded-Book.woff
 ┣ 📜iCielGothamRounded-Book.woff2
 ┣ 📜iCielGothamRounded-BookItalic.eot
 ┣ 📜iCielGothamRounded-BookItalic.svg
 ┣ 📜iCielGothamRounded-BookItalic.ttf
 ┣ 📜iCielGothamRounded-BookItalic.woff
 ┣ 📜iCielGothamRounded-BookItalic.woff2
 ┣ 📜iCielGothamRounded-Light.eot
 ┣ 📜iCielGothamRounded-Light.svg
 ┣ 📜iCielGothamRounded-Light.ttf
 ┣ 📜iCielGothamRounded-Light.woff
 ┣ 📜iCielGothamRounded-Light.woff2
 ┣ 📜iCielGothamRounded-LightItalic.eot
 ┣ 📜iCielGothamRounded-LightItalic.svg
 ┣ 📜iCielGothamRounded-LightItalic.ttf
 ┣ 📜iCielGothamRounded-LightItalic.woff
 ┣ 📜iCielGothamRounded-LightItalic.woff2
 ┣ 📜iCielGothamRounded-Medium.eot
 ┣ 📜iCielGothamRounded-Medium.svg
 ┣ 📜iCielGothamRounded-Medium.ttf
 ┣ 📜iCielGothamRounded-Medium.woff
 ┣ 📜iCielGothamRounded-Medium.woff2
 ┣ 📜iCielGothamRounded-MediumItalic.eot
 ┣ 📜iCielGothamRounded-MediumItalic.svg
 ┣ 📜iCielGothamRounded-MediumItalic.ttf
 ┣ 📜iCielGothamRounded-MediumItalic.woff
 ┣ 📜iCielGothamRounded-MediumItalic.woff2

 in font.face.css
 ![Fonts](/assets/images/font-face.png)


## Writing content

After the `init` is complete, you can see the file list in the `./docs` subdirectory.

- `index.html` as the entry file
- `README.md` as the home page
- `.nojekyll` prevents GitHub Pages from ignoring files that begin with an underscore

You can easily update the documentation in `./docs/README.md`, of course you can add [more pages](more-pages.md).

## Preview your site

Run the local server with `docsify serve`. You can preview your site in your browser on `http://localhost:3000`.

```bash
docsify serve docs
```

?> For more use cases of `docsify-cli`, head over to the [docsify-cli documentation](https://github.com/docsifyjs/docsify-cli).

## Manual initialization

If you don't like `npm` or have trouble installing the tool, you can manually create `index.html`:

```html
<!-- index.html -->

<!DOCTYPE html>
<html>
<head>
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <meta charset="UTF-8">
  <link rel="stylesheet" href="//unpkg.com/docsify/themes/vue.css">
</head>
<body>
  <div id="app"></div>
  <script>
    window.$docsify = {
      //...
    }
  </script>
  <script src="//unpkg.com/docsify/lib/docsify.min.js"></script>
</body>
</html>
```

If you installed python on your system, you can easily use it to run a static server to preview your site.

```bash
cd docs && python -m SimpleHTTPServer 3000
```

## Loading dialog

If you want, you can show a loading dialog before docsify starts to render your documentation:

```html
  <!-- index.html -->

  <div id="app">Please wait...</div>
```

You should set the `data-app` attribute if you changed `el`:

```html
  <!-- index.html -->

  <div data-app id="main">Please wait...</div>

  <script>
    window.$docsify = {
      el: '#main'
    }
  </script>
```
