# Custom OpenAPI Generator Templates

This directory is used to store custom [Mustache](https://mustache.github.io/) templates to override the default templates provided by `openapi-generator`.

## Purpose

By placing a template file in this directory with the same name as a default template, you can customize the generated code. This is useful for:

*   Adding custom logic to model classes.
*   Modifying the structure of API methods.
*   Changing the generated documentation.

## Usage

The `openapitools.json` configuration file is already set up to use this directory via the `templateDir` property:

```json
"templateDir": "./my-templates"
```

To override a template, find the original template file in the `openapi-generator` source code (or JAR file) and place a modified version with the same name here. For example, to customize how Python models are generated, you could add a `model.mustache` file to this directory.