---
description: Create an Angular application.
---

# generate application

### Overview

`ng generate application <schematic> <name> [options]` or `ng g app <schematic> <name> [options]` generates application.

### Arguments

`schematic` \(optional\)  
The schematic or collection:schematic to generate.

`name` \(required\)  
The name of the application.

### Options

`--dry-run` \(alias `-d`\)   
Run through without making any changes. 

`--force` \(alias `-f`\)   
Forces overwriting of files. 

`--inline-style` \(alias `-s`\)   
Specifies if the style will be in the ts file. 

`--inline-template` \(alias `-t`\)   
Specifies if the template will be in the ts file. 

`--prefix` \(`-p`\)   
The prefix to apply to generated selectors. 

`--routing`   
Generates a routing module. 

`--skip-package-json`   
Do not add dependencies to package.json. 

`--skip-tests` \(alias `-S`\)   
Skip creating spec files. 

`--style`   
The file extension to be used for style files. 

`--view-encapsulation`   
Specifies the view encapsulation strategy.

### Example

```bash
ng generate application my-app
```

