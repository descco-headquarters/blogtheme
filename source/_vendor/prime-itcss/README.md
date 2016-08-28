# Prime ITCSS

[![licence mit](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](http://hemersonvianna.mit-license.org/)
[![issues](https://img.shields.io/github/issues/prime-solutions/prime-itcss.svg?style=flat-square)](https://github.com/prime-solutions/prime-itcss/issues)
[![GitHub release](https://img.shields.io/github/release/prime-solutions/prime-itcss.svg?style=flat-square)](https://github.com/prime-solutions/prime-itcss/releases)
[![npm](https://img.shields.io/npm/dt/prime-itcss.svg?style=flat-square)](https://www.npmjs.com/package/prime-itcss)
[![devDependency Status](https://img.shields.io/david/dev/prime-solutions/prime-itcss.svg?style=flat-square)](https://david-dm.org/prime-solutions/prime-itcss#info=devDependencies)

## Translations

* [Portuguese - Brazil](translations/pt_BR)

## Introduction

With the intention of having a CSS core of several projects in one place. It was created this project to serve as the basis of a front-end project. Using the methodology of [ITCSS](http://itcss.io/) and syntax [SCSS](http://sass-lang.com/), [STYLUS](https://learnboost.github.io/stylus/) and [LESS](http://lesscss.org/).

The idea of using the core is when you need more than one project in the same domain. Say in your domain , you need to have the files for site and admin area. Thus, the structure with the core would look like the example below:

```
>source
 > prime
 > admin
  > style.scss 
 > site
  > style.scss 
```

With this, in the `prime` were the tools that will be used in both projects (icons, mixins, functions and more). 

## Example usage

In each project folder, it is not necessary to have some folders (`00-settings, 01-tools, 03-generic, 03-base, 04-vendor e 09-trumps`), but this is not a rule, you will know the best for your project. 

When writing , I am considering that the sample projects (site, admin), they are different and to have this distinction, folders (`05-objetcs, 06-components, 07-pages e 08-theme`), will be customized for each project.

Recalling once again, the intention is to show the concept that one must have a `prime`, to avoid repeated code and making it difficult to maintain. The organization of folders in the projects , is at the discretion of the need of the same.

`style.scss` (site)

```
@import "../prime/00-settings/_variables";
@import "../prime/01-tools/_mixins";

@import "05-objects/_alerts";

```

## Observations and Installation

The project comes with usage tips with [GulpJS](http://gulpjs.com/) or [GruntJS](http://gruntjs.com/). Choosing a automizador tasks, just knowing that only need to be aware in 3 places:

- At the root, `Gruntfile.js` or `Gulpfile.js`.
- In folder `tasks`, where tasks are divided by automator.
- In the file `package.json`, where are the dependencies.

Only interests the files , they are in the folder `source`. Opting to use one of the suggested Automation , just stay tuned to the three places that were mentioned above and run in the terminal:

```
npm install // To install the dependencies
```

And with the dependencies installed , the command `default` the automator.

## Contributing

- Fork it!
- Create your feature branch: `git checkout -b my-new-feature`
- Commit your changes: `git commit -m 'Add some feature'`
- Push to the branch: `git push origin my-new-feature`
- Submit a pull request

## Log

Check [Releases](https://github.com/prime-solutions/prime-itcss/releases) for detailed changelog.

## License

[MIT license](http://hemersonvianna.mit-license.org/) © Hemerson Vianna
