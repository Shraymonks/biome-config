# @shraymonks/biome-config

A shared [Biome](https://biomejs.dev/) configuration for consistent code style,
formatting, and linting across my projects.

## Overview

[Biome](https://biomejs.dev/) is an extremely fast toolchain for the web,
designed to replace ESLint, Prettier, and more. This repository centralizes the
configuration for Biome's linter and formatter to ensure uniformity and maintain
high code quality standards.

## Installation

To use this shared configuration, you'll need to install it alongside Biome.

First, add Biome to your project if you haven't already:

```shell
pnpm add -D @biomejs/biome
```

Next, install this shared configuration package:

```shell
pnpm add -D @shraymonks/biome-config
```

## Usage

Once the package is installed, create a `biome.json` file in the root of your
project and extend this configuration.

```json
{
  "extends": ["@shraymonks/biome-config"]
}
```

### Overriding Rules

If you need to override any rules for a specific project, you can do so directly
in your `biome.json` file. The local configuration will always take precedence.

```json
{
  "extends": ["@shraymonks/biome-config"],
  "formatter": {
    "indentStyle": "tab"
  }
}
```
