---
description: Missing command line interface documentation for Angular
---

# Angular CLI

### What Is Angular CLI?

Angular CLI is a command-line interface \(CLI\) to automate your development workflow. It allows you to:

* create a new Angular application
* run a development server with LiveReload support to preview your application during development
* add features to your existing Angular application
* run your application’s unit tests
* run your application’s end-to-end \(E2E\) tests
* build your application for deployment to production.

### Prerequisites {#prerequisites}

Both the CLI and generated project have dependencies that **require** `Node 8.9` or higher, together with `NPM 5.5.1` or higher.

You can download the latest version of Node.js for your operating system and consult the latest installation instructions on the [official Node.js website](https://nodejs.org/).

If you already have Node.js and npm installed, you can **verify** their version by running:

```bash
$ node -v  # -> displays your Node.js version
$ npm -v   # -> displays your npm version
```

### Getting Started

To install the Angular CLI:

```bash
$ npm install -g @angular/cli@latest
```

or

```bash
$ yarn global add @angular/cli@latest
```

Then make sure that it’s installed on your system and prints out version 6.0 or greater.

```bash
$ ng --version
```

![](.gitbook/assets/ng-version%20%281%29.png)

### Usage

```text
$ ng help
```

**Generating and serving an Angular project via a development server.**  
[Create](commands/ng-new.md) and [run](commands/ng-serve.md) a new project:

```bash
$ ng new my-project
cd my-project
ng serve
```

Navigate to [http://localhost:4200/](http://localhost:4200/). The app will automatically reload if you change any of the source files.

You can configure the default HTTP host and port used by the development server with two command-line options :

```bash
$ ng serve --host 0.0.0.0 --port 4201
```

