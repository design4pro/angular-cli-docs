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

### 

