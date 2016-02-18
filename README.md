JSPM ES6 boilerplate with Live reload support.
=============================================

A no nonsense jspm-es6 boilerplate for starting a minimal frontend application with live reload.

----------------
Features
-----------
- ES6 - using babel/traceur (jspm)
- JSPM - for module loading
- SASS
- Live Reload ( via browser-sync using npm scripts)

Doesn't Use Gulp or any task runner. Thanks to awesome JSPM :)

-------------------
Steps
-----
1. Clone the repo
2. npm install
3. npm install -g jspm
4. jspm install


- To start the app in development mode (No bundling)

  `npm run serve`

  This launches a development server from browser-sync and watches for any change in files

  For managing dependencies,css,etc use jspm


- For production build

  `npm run bundle`

  This creates a bundle file in `bundle/` which is injected in config by jspm.
  So now jspm uses the bundled file to load the frontend app.

  Hence the file system structure remains same for both production and development .. Jspm handles both the workflows seamlessly.
--------------

Notes
------
1. The files like JS, CSS,etc which are to be bundled go inside `src/` and are managed using jspm's `import` and module loaders .

2. The files like images, assets , html views ,etc which are not to be bundled along are to be kept in `assets/`.

Thus, when we run npm run bundle it only creates a bundle of the files in `src`


-------------
I hope this boilerplate serves u well  :D
