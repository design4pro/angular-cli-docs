---
description: Missing command line interface documentation for Angular
---

# Angular CLI

#### Overview

The Angular CLI is a tool to initialize, develop, scaffold and maintain [Angular](https://angular.io/) applications.

#### Getting Started

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

Generating and serving an Angular project via a development server [Create](commands/ng-new.md) and [run](commands/ng-serve.md) a new project:

```bash
ng new my-project
cd my-project
ng serve
```

Navigate to [http://localhost:4200/](http://localhost:4200/). The app will automatically reload if you change any of the source files.

