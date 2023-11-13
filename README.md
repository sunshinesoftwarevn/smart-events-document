# Getting started with Matbao.ws - Smart Event

event.matbao.ws is a website that provides smart event solutions in Vietnam. We offer comprehensive solutions, from planning, organizing to managing events, helping customers save time, cost and improve the effectiveness of events.

![MatBao Welcome](/assets/images/bg-ws.png)

## Environment

Prerequisites
Before proceeding, ensure you have the following installed on your system:

Operating System: Windows 10, macOS, or Linux
Node.js: Version 16 or higher
npm: Node Package Manager, included with Node.js installation
Text Editor: A code editor like Visual Studio Code, Sublime Text, or Atom
Installing Node.js and npm
Download the appropriate Node.js installer for your operating system from the official Node.js website: https://node.js.org/en/download/
Run the downloaded installer and follow the prompts to complete the installation.
Verify the Node.js installation by opening a terminal window and typing node -v. This should display the installed Node.js version.
Similarly, verify the npm installation by typing npm -v. This should display the installed npm version.
Installing ReactJS
Open a terminal window and navigate to the project directory where you want to install ReactJS.
Use the following command to install ReactJS globally:

```bash
npm install -g react react-dom
```

To verify the ReactJS installation, type the following command:

```bash
react-scripts --info
```


This should display information about the installed ReactJS CLI.

Creating a ReactJS Project
Create a new directory for your ReactJS project.
Open a terminal window and navigate to the newly created project directory.
Initialize a new ReactJS project using the following command:

```bash
npx create-react-app my-react-app
```


To install packages, run:

```bash
npm install
```

Starting the ReactJS Development Server
Navigate to the project directory using a terminal window.
Start the ReactJS development server using the following command:

```bash
npm start
```


This will start the development server and open the ReactJS application in your default browser.
If you see this page, this source is running successfully.

![MatBao Login Page](/assets/images/login.png)

## Initialize

```bash
npm i docsify-cli -g
```

If you want to write the documentation in the `./docs` subdirectory, you can use the `init` command.

```bash
docsify init ./docs
```

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
