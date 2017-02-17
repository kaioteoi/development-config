# development-config
Util development configuration that includes CSS styles pre-compiler and scripts minification, also with LiveReload feature for real time browser reload.

## IMPORTANT
### Livereload
In order to synchronize your code update with your browser, don't forget to add the **[Livereload extension](http://livereload.com/extensions/)** to your browser.

## Folder structure

In this configuration there is a pre-set __/src__ folder structure as follows:
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
After running the **"build"** task, automatically the __/dist__ folder will be created right in your __/root__, following the same __/src__ structure (except for __/scss__ that we'll keep only locally).

Feel free to rename or update the folder structure, don't forget to update the directory reference in **gulpfile.js**.
