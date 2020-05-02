<!-- @head-content@ -->
# laplacian/project.schema-model

A model which expresses the logical structure of laplacian-based projects and modules.


*Read this in other languages*: [[日本語](README_ja.md)] [[简体中文](README_zh.md)]
<!-- @head-content@ -->

<!-- @toc@ -->
## Table of contents
1. [Usage](#Usage)
1. [Index](#Index)


<!-- @toc@ -->

<!-- @main-content@ -->
## Usage

To apply this domain-model module, add the following entry to your project definition.
```yaml
project:
  domain-models:
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
- [src/entities/laplacian/document_section.yaml](<./src/entities/laplacian/document_section.yaml>)
- [src/entities/laplacian/document.yaml](<./src/entities/laplacian/document.yaml>)
- [src/entities/laplacian/module.yaml](<./src/entities/laplacian/module.yaml>)
- [src/entities/laplacian/project/examples.yaml](<./src/entities/laplacian/project/examples.yaml>)
- [src/entities/laplacian/project_type.yaml](<./src/entities/laplacian/project_type.yaml>)
- [src/entities/laplacian/project.yml](<./src/entities/laplacian/project.yml>)
- [src/entities/laplacian/source_repository.yaml](<./src/entities/laplacian/source_repository.yaml>)


<!-- @main-content@ -->