---
name: Imports
description: Use Toggled's Collection of Custom Blocks
---

# Importing Custom Blocks

With Toggled, you can import external custom blocks. (We recommend this for advanced users only.)

You can import custom blocks the same way you would import a function in static JavaScript.

```js
import { BLOCK } from 'URL'
```

You can also import a package via its name. Like this:

```js
import { BLOCK } from 'Package_Name'
```

(The package must be registered in the Toggled Package Registry. See more at https://www.npmjs.com/package/toggled-cli.) 

Once you have imported a block, you can call it just like a normal HTML block.

```html
<BLOCK></BLOCK>
```

# Design Custom Blocks

If you would like to design custom blocks for you or others to import you must do the following

### 1. Create A JS File (Vanilla JS)

For example objects.js

### 2. Create A Block

For simplicity, you create a block the same way you create a JavaScript function.

```js
export const BLOCKNAME = (e) => {
  //e is the parent element of the block access dataset via e.dataset
  const blockCode = `<p>Hello World</p>`;

  return blockCode;
};
```

You must return the block in an HTML format readable by the browser.

### 3. Configuring Your Server

Toggled will send requests to the URL hosting your custom blocks. You must ensure that you allow the following sites external script and CORS access to your site.

- toggled.tech
- www.toggled.tech
- api.toggled.tech
- backup.toggled.tech

Thanks for creating custom blocks with Toggled. If you come up with a great idea, drop us a line and we might implement it.
