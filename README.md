# development-config
Util development configuration that includes CSS styles pre-compiler and scripts minification, also with LiveReload feature for real time browser reload.

## IMPORTANT
### Livereload
In order to synchronize your code update with your browser, don't forget to add the **[Livereload extension](http://livereload.com/extensions/)** to your browser.

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
