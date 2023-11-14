## Environment

### Installation

Prerequisites
Before proceeding, ensure you have the following installed on your system:

Operating System: Windows 10, macOS, or Linux
Node.js: Version 16 or higher
npm: Node Package Manager, included with Node.js installation
Text Editor: A code editor like Visual Studio Code, Sublime Text, or Atom
Installing Node.js and npm
Download the appropriate Node.js installer for your operating system from the official Node.js website: https://node.js.org/en/download/
Run the downloaded installer and follow the prompts to complete the installation.
Verify the Node.js installation by opening a terminal window and typing node - v.This should display the installed Node.js version.
    Similarly, verify the npm installation by typing npm - v.This should display the installed npm version.
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

### API & Environment

To set up an environment, please configure it in src/configs/environment/index.js via:
📦configs
 ┣ 📂environment
 ┃ ┗ 📜index.js
 ┣ 📂theme
 ┃ ┗ 📜themeVariables.js
 ┣ 📜api.js
 ┣ 📜contants.js
 ┣ 📜dirUpload.js
 ┗ 📜themeConfig.js

![Environment Setup](/assets/images/environment.png)

```bash
ENV_ENVIRONMENT_BASE_URL_API
```
-> URL of the API domain

```bash
ENV_ENVIRONMENT_awsKeys
```

-> Config S3 upload images


### Terminology

#### State in React:
**A state** is a variable that exists inside a component, that cannot be accessed and modified outside the component, and can only be used inside the component. Works very similarly to a variable that is declared inside a function that cannot be accessed outside the scope of the function in normal javascript. State Can be modified using this.setState. The state can be asynchronous. Whenever this.setState is used to change the state class is rerender itself. Let’s see with the help of an example: 

#### Props in React:
React allows us to pass information to a Component using something called **props** (which stands for properties). Props are objects which can be used inside a component. Sometimes we need to change the content inside a component. Props come to play in these cases, as they are passed into the component and the user..


