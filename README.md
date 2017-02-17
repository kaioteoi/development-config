# development-config
Util development configuration that includes CSS styles pre-compiler and scripts minification, also with LiveReload feature for real time browser reload.

## Pre-requisites
### NodeJS and NPM
There's recommended yo have **[Node JS](https://nodejs.org/en/)** installed in your computer, we'll use a feature from node: the **[Node Package Manager (npm)](https://www.npmjs.com/)** to download all package dependencies used in daily web development.

[Click here](https://nodejs.org/en/download/) for NodeJS download.

After downloading and finishing the installation, test node in your terminal by typing `node -v`.
The current installed version should be displayed.

We can repeat this step for NPM typing `npm -v`.

### Gulp
After having **npm** installed and tested, open your terminal and type `npm install -g gulp` to install globally [Gulp](http://gulpjs.com/), our development workflow tool.

### Livereload
In order to synchronize your code update with your browser, don't forget to add the **[Livereload extension](http://livereload.com/extensions/)** to your browser.

## Usage

* If you have installed **Git Bash** use `git clone` to download config files to your computer.
Or simply [click here](https://github.com/kaioteoi/development-config/archive/master.zip) to download direct from my repo.
* Then, copy **package.json** and **gulpfile.js** in your project root directory.
* Now in your terminal, access your project folder and type `npm install` to download and install all dev dependencies listed in our **package.json**.
* After download finishing, use the command `gulp watch` in your terminal
* To active **Livereload** in your browser, open your project file in browser and click once on **livereload extension icon**.
* Happy coding !

## Folder structure

In this configuration there is a pre-set _/src_ folder structure as follows:
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
After running the **"build"** task, automatically the _/dist_ folder will be created right in your _/root_, following the same _/src_ structure (except for _/scss_ that we'll keep only locally and send only _/css_ compiled files for any deployment).

Feel free to rename or update the folder structure, don't forget to update the directory reference in **gulpfile.js**.
