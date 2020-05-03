<!-- @head-content@ -->
# laplacian/project.schema-model

This model represents the logical structure of a *Laplacian*-based project.


*Read this in other languages*: [[日本語](README_ja.md)] [[简体中文](README_zh.md)]
<!-- @head-content@ -->

<!-- @toc@ -->
## Table of contents
1. [Overview](#Overview)
1. [Usage](#Usage)
1. [Index](#Index)


<!-- @toc@ -->

<!-- @main-content@ -->
## Overview


### Model overview


The following diagram explains the entities included in this module and the relationship
between them.
![](./doc/image/model-diagram.svg)
### The list of entities


- [**Document**](<./doc/entities/Document.md>)
document
- [**Section**](<./doc/entities/Section.md>)
section
- [**Module**](<./doc/entities/Module.md>)
module
- [**Project**](<./doc/entities/Project.md>)
project
- [**ProjectType**](<./doc/entities/ProjectType.md>)
project_type
- [**Script**](<./doc/entities/Script.md>)
script
- [**ScriptOption**](<./doc/entities/ScriptOption.md>)
script_option
- [**SourceRepository**](<./doc/entities/SourceRepository.md>)
source_repository

## Usage

To apply this Model module, add the following entry to your project definition.
```yaml
project:
  models:
  - group: laplacian
    name: project.schema-model
    version: 1.0.0
```

You can run the following command to see a list of resources affected by the application of this module and their contents.
```console
$ ./script/generate --dry-run

diff --color -r PROJECT_HOME/.NEXT/somewhere/something.md PROJECT_HOME/somewhere/something.md
1,26c1,10
< content: OLD CONTENT
---
> content: NEW CONTENT
```

If there is no problem, execute the following command to reflect the change.
```console
$ ./script/generate --dry-run

```


## Index


### Source code list


- [model/project.yaml](<./model/project.yaml>)
- [src/entities/document_section.yaml](<./src/entities/document_section.yaml>)
- [src/entities/document.yaml](<./src/entities/document.yaml>)
- [src/entities/module.yaml](<./src/entities/module.yaml>)
- [src/entities/project/examples.yaml](<./src/entities/project/examples.yaml>)
- [src/entities/project_type.yaml](<./src/entities/project_type.yaml>)
- [src/entities/project.yml](<./src/entities/project.yml>)
- [src/entities/script_option.yaml](<./src/entities/script_option.yaml>)
- [src/entities/script.yaml](<./src/entities/script.yaml>)
- [src/entities/source_repository.yaml](<./src/entities/source_repository.yaml>)


<!-- @main-content@ -->