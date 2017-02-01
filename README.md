# breakdance [![NPM version](https://img.shields.io/npm/v/breakdance.svg?style=flat)](https://www.npmjs.com/package/breakdance) [![NPM monthly downloads](https://img.shields.io/npm/dm/breakdance.svg?style=flat)](https://npmjs.org/package/breakdance)  [![NPM total downloads](https://img.shields.io/npm/dt/breakdance.svg?style=flat)](https://npmjs.org/package/breakdance) [![Linux Build Status](https://img.shields.io/travis/breakdance/breakdance.svg?style=flat&label=Travis)](https://travis-ci.org/breakdance/breakdance)  [![Build Status](https://img.shields.io/travis/breakdance/breakdance.svg?style=flat)](https://travis-ci.org/breakdance/breakdance)

> Breakdance is a node.js library for converting HTML to markdown. Highly pluggable, flexible and easy to use. It's time for your markup to get down.

Breakdance is a node.js library for converting HTML to markdown. You can use breakdance to:

* Migrate HTML blog posts to markdown
* Convert wiki pages to markdown
* Convert HTML documentation to markdown
* Convert HTML presentations or slide decks to markdown
* Convert busy web pages into readable markdown documents.

Visit [breakdance.io](http://breakdance.io) for detailed documentation, [examples](http://breakdance.io/examples), [recipes](http://breakdance.io/recipes), and advice on [authoring and finding plugins](http://breakdance.io/plugins.html).

## What's different about breakdance?

Breakdance uses [cheerio](https://github.com/cheeriojs/cheerio) to parse HTML, and [snapdragon](https://github.com/jonschlinkert/snapdragon) for rendering, which provides granular control over the entire conversion process in a way that is easy to understand, reason about, and [customize](http://breakdance.io/plugins.html).

**Generates well-formatted markdown**

* Comprehensive [HTML tag coverage](lib/compile.js).
* Granular control over every HTML element and attributes
* Even **converts HTML tables** to markdown!

**Extremely pluggable**

Every part of the conversion is customizable:

* [options](http://breakdance.io/plugins.html) are available for customizing output of any HTML tag if you don't like the defaults
* [plugins](http://breakdance.io/plugins.html) are easy to write if you'd like to share your customizations with the world

## HTML-to-markdown example

**Tables**

The following HTML table:

```html
<table>
  <thead>
    <tr>
      <th>Heading 1</th>
      <th>Heading 2</th>
      <th>Heading 3</th>
      <th>Heading 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Table cell</td>
      <td>Table cell</td>
      <td>Table cell</td>
      <td>Table cell</td>
    </tr>
    <tr>
      <td>Table cell</td>
      <td>Table cell</td>
      <td>Table cell</td>
      <td>Table cell</td>
    </tr>
  </tbody>
</table>
```

Would render to the following markdown:

```html
| Heading 1 | Heading 2 | Heading 3 | Heading 4 | 
| --- | --- | --- | --- | 
| Table cell | Table cell | Table cell | Table cell | 
| Table cell | Table cell | Table cell | Table cell | 
```

See [the documentation](http://breakdance.io/examples.html) for more examples.

## About

### Community

Get updates on Breakdance's development and chat with the project maintainers and community members.

* Implementation help may be found at Stack Overflow (please use the tag [breakdance](https://stackoverflow.com/questions/tagged/breakdance)`breakdance`).
* For maximum discoverability, plugin developers should use the keyword `breakdance` on packages which modify or add to the functionality of Breakdance when distributing through [npm](https://www.npmjs.com/browse/keyword/breakdance) or similar delivery mechanisms.

### Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

Please read the [contributing guide](.github/contributing.md) for advice on opening issues, pull requests, and coding standards.

### Running tests

Install dev dependencies:

```sh
$ npm install && npm test
```

### Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](https://twitter.com/jonschlinkert)

### License

Copyright © 2017, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT license](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.4.2, on January 31, 2017._