# Creating Mods

<span style="color: #419c59;">**NOTE:**</span> This page was made for JET versions 1.1.1 and prior. If you are using a newer version, the mod loader has been rewritten, and a new documentation has yet to be drafted for it.

Mods should be placed in your `JET/Server/user/mods` directory. A mod folder usually follows this structure:

```
Author-MyMod-1.0.0/
|
|__mod.config.json
|__src/
|  |__ ... scripts go here ...
|  |__ ...
```

The most important file for your mod to load properly is your **mod.config.json**. This configuration file should be structured similar to below:

```js
{
	"name": "ExamineAll",
	"author": "TheMaoci",
	"version": "1.0.0",
	"license": "MIT",
	"src": {
		"src/ScriptToLoad_1.js": "TamperModLoad",
		"src/ScriptToLoad_2.js": "CacheModLoad"
	}
}
```

## Script Loading Methods

When declaring a script to be loading in your **mod.config.json**, you can load it either with `TamperModLoad` or `CacheModLoad`.

- `TamperModLoad` loads a mod just before the server starts so all classes, variables, etc. are already loaded and accessible.
- `CacheModLoad` loads a mod just after caching is completed.

## Script Structure

```js
// src/myscript.js

exports.mod = (mod_info) => {
    // Your script logic goes here. 
    // mod_info contains the mod.config.json file as a JavaScript object.
}
```