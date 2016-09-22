## NPM

Vomit has been built with modularity in mind and for this reason, it is recommended to use NPM has the primary installation method. Vomit's code follows CommonJS standards and pairs nicely with module bundler such as Browserify or Webpack

```shell
# latest stable
$ npm install vomit
```

## CLI

Vomit also comes with tools to test, visualize and author components. Using NPM, you can install the cli `vomit` with a simple command:

```shell
# install cli
$ npm install -g vomit

# display vomit cli help
$ vomit --help
```

## Standalone

If you don't use modules bundler, you can include vomit as a global variable by downloading the standalone version and include it with a script tag:

<a href="https://github.com/bredele/vomit/blob/master/dist/vomit.js" target="_blank">Development version</a>
<a href="https://github.com/bredele/vomit/blob/master/dist/vomit.min.js" target="_blank">Production version</a>

## Bower

Vomit is also available on Bower registry.

```shell
# latest stable
$ bower install vomit
```

## Dev Build

```shell
git clone https://github.com/bredele/vomit.git
cd vomit
npm install
npm run build
```

Important: the command `npm run build` can be used with your continuous integration tools in order to build your own version of Vomit.