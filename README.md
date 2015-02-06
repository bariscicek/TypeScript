TypeScript ExtJS Emitter
======================

A fork of Typescript 1.4 that emits classes in a way that ExtJS understands.

##Why?

The Javascript emitted by the Typescript compiler is not compatible with the ExtJS class system. ExtJS requires classes to be defined using syntax like `Ext.define(CLASSNAME, MEMBERS);` but Typescript emits code based around prototypes.

This forked compiler emits code that looks just like the ExtJS classes you would write in regular Javascript.

##ExtJS API Type Declarations

To get the most use out of this compiler you will also need some type declarations (*.d.ts files) for the ExtJS API. There is a companion project to provide these: https://github.com/Dretch/typescript-declarations-for-ext

##Screenshot
![ScreenShot](https://raw.github.com/fabioparra/TypeScriptExtJSEmitter/master/TypeScriptExtJSEmitter/images/screenshot.jpg)

##Demo

https://rawgithub.com/fabioparra/TypeScriptExtJSEmitter/master/TypeScriptExtJSEmitter/index.html

##Compatability

This project is compatible with Typescript 1.4 and ExtJS 3, 4 and 5. The emitted classes can be processed by Sencha CMD.

##Usage with Visual Studio 2013

####Update tsc.js and typescriptServices.js files (used by visual studio editor and msbuild tasks )

- Install vs 2013 plugin: https://visualstudiogallery.msdn.microsoft.com/2d42d8dc-e085-45eb-a30b-3f7d50d55304
- Download latest modified compiler: https://github.com/fabioparra/TypeScript/releases/tag/v1.4
- Run copy_to_vs2013.bat file as administrator
