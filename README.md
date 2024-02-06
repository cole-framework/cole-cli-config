# Project Configuration for Cole CLI

This repository contains configuration files for the Cole CLI, a tool for simplifying the setup and generation of web applications using clean architecture principles. The configuration files provided here help customize the behavior of the CLI.

## Configuration Files

### Primary Configuration (primary.config.json)

- **Version**: The version of the configuration (e.g., "0.0.0").
- **Languages**: Define the programming languages supported by the CLI, along with their dependencies and aliases. Each language entry specifies:
  - Name
  - Package name
  - Alias
  - Dependencies (for TypeScript or JavaScript)
  - Cole Plugin (for code generation)
  - Cole CLI Plugin (for CLI behavior)
  - Supported data types

### Web Frameworks

Define the web frameworks supported by the CLI. Each framework entry specifies:

- Name
- Alias
- Package name
- Dependencies (for TypeScript or JavaScript)

### Databases

Define the databases supported by the CLI. Each database entry specifies:

- Name
- Alias
- Package name
- Case style (e.g., "snake_case" for mapping)
- Dependencies (for TypeScript or JavaScript)
- Data type mappings (for TypeScript)
- Cole Plugin (for code generation)

## Usage

To use these configuration files with Cole CLI, simply invoke the CLI commands without specifying a configuration file path. The CLI will automatically download the latest configuration files from this repository.

For example, to initialize a new project using TypeScript and Express.js with MongoDB as the database:

```bash
cole new project -n "NewProject" -l "typescript" -f "express" -d "mongo"
```
