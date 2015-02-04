# Ðapp styles
*Version 0.1*

These styles give a simple basic layout for your Ðapps.

## Setup


### CSS
To use it as CSS file just link the css file from the `dist/` folder.


### LESS
To use it as less file, which would allow you to overwrite all constants 
from the `constant.import.less` and use the mixins from `mixins.import.less`.
Just link the `dapp-styles.less` in your apps main less file.

### Meteor
To use it in a Meteor app add the `less` package:

    $ meteor add less

Copy this dapp-styles repo content into your apps `public` folder under `public/dapp-styles/`
and link to the `dapp-styles.less` in the main less files of your project with:

    @import 'public/dapp-styles/dapp-styles.less';



## Usage

The main layout consists of the following HTML elements:

```html

<header class="dapp-header">
    
</header>

<div class="dapp-flex-content">
    
    <!-- aside -->
    <aside class="dapp-aside">

    </aside>

    <!-- content-->
    <main class="dapp-content">
        
    </main>

    <!-- actionbar -->
    <aside class="dapp-actionbar">

    </aside>

</div>

<!-- footer -->
<footer class="dapp-footer">
    
</footer>

```

This gives you a basic flex box layout with a fixed header height and footer height, and a growable content area.

You can remove any part (header, footer, asides) of it and still have nice fitting containers.

### Using overflow auto in containers

If you want the apps area to be maximal the window size and the content of your containers to be `overflow: auto`,
just add the `dapp-overflow` class to the `dapp-header`, `dapp-content`, `dapp-footer`, `dapp-actionbar` and/or `dapp-aside` containers and add the following to your main CSS file:

```css
html, body {
    height: 100%;
}
```

### Mixins

When you use the less version, of the framework then you will be able
to use all its LESS mixins including the LESSHAT mixins (https://github.com/madebysource/lesshat, which are used by the dapp-styles) in your own LESS files.

### Elements

TODO


