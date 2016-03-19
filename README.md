## Easystatic - static site generator

> The easiest way to generate a static website for your project. It uses [Markdown It](https://markdown-it.github.io/)
> for web pages, [EJS](http://ejs.co/) and [Postcss](http://postcss.org/) for site layout, [Browsersync](https://browsersync.io/)
> as a development server, allowing "live editing" and testing the site on all connected-devices.

### Why use Easystatic?

1. It advocates convention over configuration
2. It's JavaScript-based, cross-platform, no need to have Ruby/Go/PHP installed
3. It's build top of the modern mainstream front-end dev tools such as [Babel](https://babeljs.io),
   [Postcss](http://postcss.org/), [Browsersync](https://browsersync.io/)
4. It contains a build-in development server with "live reload"
5. It can scaffold the basic site layout for you

### Requirements

  * Mac OS X, Windows, or Linux
  * [Node.js](https://nodejs.org/) v5.0 or newer
  * `npm` v3.3 or newer (new to [npm](https://docs.npmjs.com/)?)
  * `node-gyp` prerequisites mentioned [here](https://github.com/nodejs/node-gyp) (optional)

### How to Install

```sh
$ npm install -g easystatic  
```

### How to Use

To build the site and launch it in a browser run:

```
$ es start <path>       # for example, `es start mysite.com`
```

..where `<path>` is the name of the directory with `.md` files, or the name of an empty folder.
Easystatic will scaffold the basic site layout for you by creating an "assets" folder with
[EJS](http://ejs.co/)-based layout template file (`assets/main.ejs`) and CSS (`assets/main.css`).
You can customize the look and feel of your site by editing layout files inside the `assets` folder.

### How to Deploy

Below is an example of how you can deploy your site to [GitHub Pages](https://help.github.com/categories/github-pages-basics/) —
a free CDN-hosting for static websites:

```sh
$ es deploy <path> --repo=<github-repository-url> --domain=<domain-name>
```

..where `<repo>` is a GitHub repository, and `<domain>` is a custom domain name
for your site. For example:

```sh
$ es deploy mysite.com --repo=username/mysite.com --domain=mysite.com
```

### Contributing

Check out [CONTRIBUTING.md](CONTRIBUTING.md) file for information on how you can contribute to this project.

### Related Projects

* [React Starter Kit](https://github.com/kriasoft/react-starter-kit) — Isomorphic web app boilerplate (Node.js/Express, React.js, GraphQL)

### Support

* [#easystatic](http://stackoverflow.com/questions/tagged/easystatic) on StackOverflow
* [#easystatic](https://gitter.im/easystatic/easystatic) on Gitter
* [@koistya](https://twitter.com/koistya) on [Codementor](https://www.codementor.io/koistya)

### Licence

Copyright © 2016 Eeasystatic [contributors](https://github.com/easystatic/easystatic/graphs/contributors).
This source code is licensed under the Apache 2.0 license found in the
[LICENSE.txt](https://github.com/easystatic/easystatic/blob/master/LICENSE.txt) file.
The documentation to the project is licensed under the [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/) license.
