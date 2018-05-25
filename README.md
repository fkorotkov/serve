# serve

[![Build Status](https://circleci.com/gh/zeit/serve.svg?&style=shield)](https://circleci.com/gh/zeit/serve)
[![Join the community on Spectrum](https://withspectrum.github.io/badge/badge.svg)](https://spectrum.chat/micro/serve)

Assuming you would like to serve a static site, single page application or just a static file (on the network or locally), this package is just the right choice for you.

It behaves exactly like static deployments on [Now](https://zeit.co/now), so it's perfect for developing your static project. Then, when it's time to push it into production, you [deploy it](https://zeit.co/docs/examples/static).

Furthermore, it also provides a neat interface for listing the directory's contents:

![screenshot](https://user-images.githubusercontent.com/6170607/40541195-167ff460-601b-11e8-8f66-3b0c7ff96cbb.png)

## Usage

Firstly, install the package from [npm](https://npmjs.com/release) (you'll need at least Node.js LTS):

```bash
npm install -g serve
```

Alternatively, you can use [Yarn](https://yarnpkg.com/en/) to install it:

```bash
yarn global add serve
```

Once that's done, you can run this command inside your project's directory:

```bash
serve [options] <path>
```

### Command Line Options

Run this command to see a list of all available options:

```bash
serve --help
```

### Configuration

To customize `serve`'s behavior, create a `serve.json` file and insert any of [these properties](https://github.com/zeit/serve-handler#options). In addition, `serve` will also detect `now.json` files if they contain the `static` property.

## API

The core of `serve` is [serve-handler](https://github.com/zeit/serve-handler), which can be used as middleware in existing HTTP servers.

## Contributing

1. [Fork](https://help.github.com/articles/fork-a-repo/) this repository to your own GitHub account and then [clone](https://help.github.com/articles/cloning-a-repository/) it to your local device
2. Uninstall `serve` if it's already installed: `yarn global remove serve`
3. Link it to the global module directory: `yarn link`

After that, you can use the `serve` command everywhere. [Here](https://github.com/zeit/serve/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+for+beginners%22)'s a list of issues that are great for beginners.

## Credits

This project used to be called "list" and "micro-list". But thanks to [TJ Holowaychuk](https://github.com/tj) handing us the new name, it's now called "serve" (which is much more definite).

## Author

Leo Lamprecht ([@notquiteleo](https://twitter.com/notquiteleo)) - [ZEIT](https://zeit.co)
