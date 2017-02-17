# development-config
Util development configuration that includes CSS styles pre-compiler and scripts minification, also with LiveReload feature for real time browser reload.

## Pre-requisites
### NodeJS and NPM
Install **[Node JS](https://nodejs.org/en/)**, we'll use **[Node Package Manager (npm)](https://www.npmjs.com/)** from it to download all packages.

**[NodeJS download](https://nodejs.org/en/download/)**

#### Testing NodeJS and npm
In your terminal type `node -v`.
The current installed version should be displayed.

We can repeat this step for NPM typing `npm -v`.

### Gulp
After installing **npm**, use the command `npm install -g gulp` to install globally **[Gulp](http://gulpjs.com/)**, our development workflow tool.

*With __gulp__ installed globally you can use `gulp` commands in any of your projects*

### Livereload
In order to synchronize your code saving with your browser reload, don't forget to add the **[Livereload extension](http://livereload.com/extensions/)** to your browser.

## Usage

* [Click here to download the configuration files directly from this repo.](https://github.com/kaioteoi/development-config/archive/master.zip)
* Copy/move **package.json** and **gulpfile.js** files to your project root directory.
* In terminal, access your project folder and use the command `npm install` to download all dev dependencies listed in **package.json**.
* Initialize gulp task using the command `gulp watch` in your terminal.
* To active **Livereload** in your browser, open your project file in browser and click once on **livereload extension icon** in right top of your browser.
* Happy coding !

## Folder structure

In this configuration there is a pre-set `/src` folder structure as follows:
```
/root
  gulpfile.js
  package.json
  /src
    /js
    /scss
    /images
    /fonts
```
After running the **"build"** task, automatically the `/dist` folder will be created right in your `/root`, following the same `/src` structure (except for `/scss` that we'll keep only locally and send only `/css` compiled files for any deployment).

Feel free to rename or update the folder structure, don't forget to update the directory reference in **gulpfile.js**.
