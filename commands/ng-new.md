# new

### Overview

`ng new [name]` creates a new angular application.

Default applications are created in a directory of the same name, with an initialized Angular application.

### Options

| Option | Alias | Description | Default |
| :--- | :--- | :--- | :--- |
| `--collection` | `-c` | Schematics collection to use. |  |
| `--directory` |  | The directory name to create the workspace in. |  |
| `--dry-run` | `-d` | Run through without making any changes. |  |
| `--force` | `-f` | Forces overwriting of files. |  |
| `--inline-style` | `-s` | Specifies if the style will be in the ts file. |  |
| `--inline-template` | `-t` | Specifies if the template will be in the ts file. |  |
| `--new-project-root` |  | The path where new projects will be created. |  |
| `--prefix` | `-p` | The prefix to apply to generated selectors. |  |
| `--routing` |  | Generates a routing module. |  |
| `--skip-git` | `-g` | Skip initializing a git repository. |  |
| `--skip-install` |  | Skip installing dependency packages. |  |
| `--skip-tests` | `-S` | Skip creating spec files. |  |
| `--style` |  | The file extension to be used for style files. | `css` |
| `--verbose` | `-v` | Adds more details to output logging. |  |
| `--view-encapsulation` |  | Specifies the view encapsulation strategy. |  |
| `--help` | `-h` | Help. |  |

### Example

```bash
ng new my-app --prefix app --style scss --skip-tests --verbose
```

### Generating

You can use the `ng generate` \(or just `ng g`\) command to generate Angular components, directives, pipes, services and more.

You can find all possible blueprints in the table below:

| Scaffold | Usage |
| :--- | :--- |
| [Component](https://github.com/angular/angular-cli/wiki/generate-component) | `ng g component my-new-component` |
| [Directive](https://github.com/angular/angular-cli/wiki/generate-directive) | `ng g directive my-new-directive` |
| [Pipe](https://github.com/angular/angular-cli/wiki/generate-pipe) | `ng g pipe my-new-pipe` |
| [Service](https://github.com/angular/angular-cli/wiki/generate-service) | `ng g service my-new-service` |
| [Class](https://github.com/angular/angular-cli/wiki/generate-class) | `ng g class my-new-class` |
| [Guard](https://github.com/angular/angular-cli/wiki/generate-guard) | `ng g guard my-new-guard` |
| [Interface](https://github.com/angular/angular-cli/wiki/generate-interface) | `ng g interface my-new-interface` |
| [Enum](https://github.com/angular/angular-cli/wiki/generate-enum) | `ng g enum my-new-enum` |
| [Module](https://github.com/angular/angular-cli/wiki/generate-module) | `ng g module my-module` |

angular-cli will add reference to `components`, `directives` and `pipes` automatically in the `app.module.ts`. If you need to add this references to another custom module, follow these steps:

1. `ng g module new-module` to create a new module
2. call `ng g component new-module/new-component`

This should add the new `component`, `directive` or `pipe` reference to the `new-module`you've created.

### Updating

To update Angular CLI to a new version, you must update both the global package and your project's local package.

Global package:

```bash
$ npm uninstall -g @angular/cli
npm cache verify
# if npm version is < 5 then use `npm cache clean`
npm install -g @angular/cli@latest
```

Local project package:

```bash
$ rm -rf node_modules dist # use rmdir /S/Q node_modules dist in Windows Command Prompt; use rm -r -fo node_modules,dist in Windows PowerShell
npm install --save-dev @angular/cli@latest
npm install
```

You can find more details about changes between versions in [the Releases tab on GitHub](https://github.com/angular/angular-cli/releases).

