# development-config
Util development configuration that includes CSS styles pre-compiler and scripts minification, also with LiveReload feature for real time browser reload.

## Folder structure

There is a pre-set for the /src folder structure.

The basic structure is as follows:
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
After running the **"build"** task, we will have a auto generated __/dist__ folder right in your __/root__, following the same __/src__ structure (regardless for __/scss__ that we'll keep only locally).

Feel free to rename or update the folder structure, don't forget to update the directory reference in **gulpfile.js**.
