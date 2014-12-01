# TypeScript & KnockoutJS TodoMVC Example

> TypeScript is a language for application-scale JavaScript development. TypeScript is a typed superset of JavaScript that compiles to plain JavaScript. Any browser. Any host. Any OS. Open Source.

> _[TypeScript - typescriptlang.org](http://typescriptlang.org)_


> Knockout.js helps you simplify dynamic JavaScript UIs using the Model-View-ViewModel (MVVM) pattern.

> _[Knockout.js - knockoutjs.com](http://knockoutjs.com)_


## Learning TypeScript

The [TypeScript website](http://typescriptlang.org) is a great resource for getting started.

Here are some links you may find helpful:

* [Tutorial](http://www.typescriptlang.org/Tutorial)
* [Code Playground](http://www.typescriptlang.org/Playground)
* [Documentation](http://typescript.codeplex.com/documentation)
* [Applications built with TypeScript](http://www.typescriptlang.org/Samples)
* [Blog](http://blogs.msdn.com/b/typescript)
* [Source Code](http://typescript.codeplex.com/sourcecontrol/latest#README.txt)

Articles and guides from the community:

* [Thoughts on TypeScript](http://www.nczonline.net/blog/2012/10/04/thoughts-on-typescript)
* [ScreenCast - Why I Like TypeScript](http://www.leebrimelow.com/why-i-like-typescripts)

Get help from other TypeScript users:

* [TypeScript on StackOverflow](http://stackoverflow.com/questions/tagged/typescript)
* [Forums](http://typescript.codeplex.com/discussions)
* [TypeScript on Twitter](http://twitter.com/typescriptlang)

_If you have other helpful links to share, or find any of the links above no longer work, please [let us know](https://github.com/tastejs/todomvc/issues)._


## Learning Knockout.js

The [Knockout.js website](http://knockoutjs.com) is a great resource for getting started.

Here are some links you may find helpful:

* [Documentation](http://knockoutjs.com/documentation/introduction.html)
* [Tutorials](http://learn.knockoutjs.com)
* [Live examples](http://knockoutjs.com/examples)

Articles and guides from the community:

* [Getting Started with Knockout.js](http://www.adobe.com/devnet/html5/articles/getting-started-with-knockoutjs.html)
* [Into the Ring with Knockout.js](http://net.tutsplus.com/tutorials/javascript-ajax/into-the-ring-with-knockout-js)
* [Beginners Guide to Knockout.js](http://www.sitepoint.com/beginners-guide-to-knockoutjs-part-1)

Get help from other Knockout.js users:

* [Knockout.js on StackOverflow](http://stackoverflow.com/questions/tagged/knockout)
* [Mailing list on Google Groups](http://groups.google.com/group/knockoutjs)
* [Knockout.js on Twitter](http://twitter.com/knockoutjs)
* [Knockout.js on Google +](https://plus.google.com/communities/106789046312204355684/stream/c5bfcfdf-3690-44a6-b015-35aad4f4e42e)

_If you have other helpful links to share, or find any of the links above no longer work, please [let us know](https://github.com/tastejs/todomvc/issues)._


## Implementation

[TypeScript](http://typescriptlang.org) is a superset of JavaScript, with optional type annotations. As any JS is valid TS, there is no interoperability issue. You could slowly convert an existing JS code-base and use JS libraries natively. You already know most of the language. It compiles back to JS.

It's attractive to people with a background in strongly typed languages, who are willing to type in more code-- classes and type annotations-- receiving the benefit of type checking on compile time. IntelliSense works better, as well.


### Editors
A great editor for TypeScript is Visual Studio 2013 with [TypeScript](http://go.microsoft.com/fwlink/?LinkID=266563) and  [Web Essentials 2013](http://visualstudiogallery.msdn.microsoft.com/07d54d12-7133-4e15-becb-6f451ea3bea6) plugins.

Webstorm has [support for TypeScript](http://blog.jetbrains.com/webstorm/2013/11/enjoy-typescript-in-webstorm/) as well.


### Ambient declarations

It is useful to have type information for the libraries you use. [DefinitelyTyped](https://github.com/borisyankov/DefinitelyTyped) is a nice collection of annotations by Boris Yankov.


### Files

* `*.ts` are source code files.
* `*.d.ts` are ambient declarations for libraries.
* `*.js` are generated by the compiler, except in the `js/libs` folder.
* `*.js.map` are [source maps](http://www.html5rocks.com/en/tutorials/developertools/sourcemaps/) generated by the compiler, for better debugging experience.
* `_all.ts` is a convention used to enumerate file references in the project for the benefit of the TypeScript compiler.

If the number of files grows, you could put an `_all.ts` file into each folder, move all nested references to it and reference the nested `_all.ts` from the parent `_all.ts`.

Start reading `TodoCtrl.ts` first, continue with `Application.ts` and `index.html`, then the rest of it is easy.


### KnockoutJS

There is very little difference between this app and the Knockout.js TodoMVC app in how KnockoutJS is used.
The only significant difference is that app, ViewModel and Model are in separate files.


## Credit

This TodoMVC application was created based on Knockout.js TodoMVC exmaple, which has been created by [ashish101](https://github.com/ashish01/knockoutjs-todos), and [Ryan Niemeyer](http://knockmeout.net).