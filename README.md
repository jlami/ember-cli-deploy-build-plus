# ember-cli-deploy-build-plus

> An ember-cli-deploy plugin to build your ember-cli application

<hr/>
**WARNING: This plugin is only compatible with ember-cli-deploy versions >= 0.5.0**
<hr/>

This plugin will build your ember-cli application files and output them to a directory.

## What is an ember-cli-deploy plugin?

A plugin is an addon that can be executed as a part of the ember-cli-deploy pipeline. A plugin will implement one or more of the ember-cli-deploy's pipeline hooks.

For more information on what plugins are and how they work, please refer to the [Plugin Documentation][1].

## Quick Start

- Install this plugin

```bash
$ ember install ember-cli-deploy-build-plus
```

- Run the pipeline

```bash
$ ember deploy
```

## Installation
Run the following command in your terminal:

```bash
ember install ember-cli-deploy-build-plus
```

## ember-cli-deploy Hooks Implemented

For detailed information on what plugin hooks are and how they work, please refer to the [Plugin Documentation][1].

- `configure`
- `setup`
- `build`

## Configuration Options

For detailed information on how configuration of plugins works, please refer to the [Plugin Documentation][1].

### environment

The environment for which you'd like to build. This relates directly to the environments in your `config/environment.js` file.

*Default:* `'production'`

### outputPath

The path to the directory you'd like the project to be built in retured to `context.distDir`.

*Default:* `tmp/deploy-dist`

### distDir

Mutable input path normally setup by outputPath where your project will be built.

*Default:* `context.distDir`

## Prerequisites

None

## Running Tests

- `npm test`

[1]: http://ember-cli.github.io/ember-cli-deploy/plugins "Plugin Documentation"
