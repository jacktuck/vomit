# vomit
 > **v**~~irtual d~~**om it** ~~sucks~~

[![vomit](http://static.tumblr.com/67e9d19760f9ab511ea7142b267a0840/etrtigr/zohmqv4pn/tumblr_static_unicornpuke.jpg)](http://requirebin.com/?gist=df0d460eb9506d5e8a17b3f33141b30b)

[![Build Status](https://travis-ci.com/bredele/vomit.svg?token=Y4CxXGeQJuzFDfs59QPR&branch=master)](https://travis-ci.com/bredele/vomit)

## Intro

Vomit is a simple function call that allows you to quickly build components that update themselves.

```js
var name = 'Nyan'
var rainbow = ['red', 'orange', 'yellow', 'green', 'blue', 'purple']

var el = vomit`<section>
  <h1>${name} the cat!</h1>
  <ul>
    ${rainbow.map(color => vomit`<li>${color}</li>`)}
  </ul>
</section>`
```

Vomit does not force you into any syntax/API but instead uses the power of JavaScript [template literals](https://developers.google.com/web/updates/2015/01/ES6-Template-Strings) built in your browser. String substitution (expression between `${}`) presents many [benefits](https://developers.google.com/web/updates/2015/01/ES6-Template-Strings) and Vomit makes it even better allowing you to substitute Objects, Arrays, DOM Elements, Functions, **Promises and even Streams**.

Check out our [5 minutes getting started](https://github.com/bredele/vomit/blob/master/doc/getting-started.md)!

Other features are:
- Component oriented development using DOM diffing based on real DOM (not virtual DOM)
- Separate and optimize rendering of static and dynamic content
- HTML5 Web Component
- Works server side
- Works with SVG
- 2kb minified + gzipped, ideal for mobile and to include as dependency

You'll find Vomit disgustingly easy to learn. Please check out [live examples]() and [docs]().

## Question

For questions and feedback please use the [Gitter chat room](). For support, bug reports and or feature requests please use the issue list of this repo and make sure it's not present yet in our [reporting checklist]().

## Contribution

Vomit is an open source project and would not exist without its community. If you want to participate please make sure to read the contributing guide before making a pull request. If you have any vomit-related project, component or other let everyone know on our [chat room]() or in our [wiki]().

## License

[![NPM](https://nodei.co/npm/vomit.png)](https://nodei.co/npm/vomit/)

The MIT License (MIT)

Copyright (c) 2016 Olivier Wietrich

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
