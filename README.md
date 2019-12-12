# My-WP-BootStrap Starter Theme with SASS and autoreload functionality using VS Code 

This is another wordpress starter theme using [Bootstrap 4](https://getbootstrap.com/), 

setup the liveSass Compiler extension, change the savePath as described bellow.

```javascript
"liveSassCompile.settings.formats":[
        // This is Default.
        {
            "format": "expanded",
            "extensionName": ".css",
            // "savePath": "/public/css"
            "savePath": "./" //changed for wordpress
        },
    ],
```
CMD+Shift+P -> Live Sass: Watch Sass


Install browser-sync npm package using the following command, in case if you have not already installed it.

```bash
npm i -g browser-sync 
```

then add package.json as follows :-

```javascript
{
    "name": "mywpbootstrapstartertheme",
    "version": "1.0.0",
    "description": "",
    "main": "index.js",
    "scripts": {
      "start": "browser-sync start --proxy 'wp5.tst' --files '**.*' "
    }
  }
  
```

in the terminal run 

```bash
npm run start
```

Enjoy