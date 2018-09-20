---
description: Missing command line interface documentation for Angular
---

# Angular CLI

The official documentation for the Angular CLI is located in this repo's [wiki](https://github.com/angular/angular-cli/wiki).

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

You can download the latest version of Node.js for your operating system and consult the latest installation instructions on the [_official Node.js website_](https://nodejs.org/).

If you already have Node.js and npm installed, you can **verify** their version by running:

{% code-tabs %}
{% code-tabs-item title="displays your Node.js version" %}
```bash
node -v
```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% code-tabs %}
{% code-tabs-item title="displays your npm version" %}
```text
npm -v
```
{% endcode-tabs-item %}
{% endcode-tabs %}

### Getting Started

To install the Angular CLI:

```bash
npm install -g @angular/cli@latest
```

or

```bash
yarn global add @angular/cli@latest
```

Then make sure that it’s installed on your system and prints out version 6.0 or greater.

```bash
ng --version
```

![](.gitbook/assets/ng-version%20%281%29.png)

### Usage

```text
ng help
```

**Generating and serving an Angular project via a development server.**  
[_Create_](commands/ng-new.md) and [_run_](commands/ng-serve.md) a new project:

```bash
ng new my-project
```

```text
cd my-project
```

```text
ng serve
```

Navigate to [_http://localhost:4200/_](http://localhost:4200/). The app will automatically reload if you change any of the source files.

You can configure the default HTTP host and port used by the development server with two command-line options :

```bash
ng serve --host 0.0.0.0 --port 4201
```

### Generating

You can use the `ng generate` \(or just `ng g`\) command to generate Angular components, directives, pipes, services and more.

You can find all possible blueprints in the table below:

| Scaffold | Usage |
| :--- | :--- |
| Application | `ng g application my-new-app` |
| Component | `ng g component my-new-component` |
| Directive | `ng g directive my-new-directive` |
| Pipe | `ng g pipe my-new-pipe` |
| Service | `ng g service my-new-service` |
| Class | `ng g class my-new-class` |
| Guard | `ng g guard my-new-guard` |
| Interface | `ng g interface my-new-interface` |
| Enum | `ng g enum my-new-enum` |
| Module | `ng g module my-module` |

angular-cli will add reference to `components`, `directives` and `pipes` automatically in the `app.module.ts`. If you need to add this references to another custom module, follow these steps:

1. `ng g module new-module` to create a new module
2. call `ng g component new-module/new-component`

This should add the new `component`, `directive` or `pipe` reference to the `new-module`you've created.

### Updating

To update Angular CLI to a new version, you must update both the global package and your project's local package.

**Global package**:

```bash
npm uninstall -g @angular/cli
```

```text
npm cache verify
```

If npm version is &lt; 5 then use `npm cache clean`

```text
npm install -g @angular/cli@latest
```

**Local project package**:

```bash
rm -rf node_modules dist
```

Use rmdir /S/Q node\_modules dist in Windows Command Prompt; use rm -r -fo node\_modules,dist in Windows PowerShell

```text
npm install --save-dev @angular/cli@latest
```

```text
npm install
```

You can find more details about changes between versions in [_the Releases tab on GitHub_](https://github.com/angular/angular-cli/releases).

