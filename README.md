oclif-demo
=================

A new CLI generated with oclif


[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-demo.svg)](https://npmjs.org/package/oclif-demo)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-demo.svg)](https://npmjs.org/package/oclif-demo)


<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g oclif-demo
$ oclif-demo COMMAND
running command...
$ oclif-demo (--version)
oclif-demo/0.0.0 darwin-arm64 node-v22.14.0
$ oclif-demo --help [COMMAND]
USAGE
  $ oclif-demo COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`oclif-demo hello PERSON`](#oclif-demo-hello-person)
* [`oclif-demo hello world`](#oclif-demo-hello-world)
* [`oclif-demo help [COMMAND]`](#oclif-demo-help-command)
* [`oclif-demo plugins`](#oclif-demo-plugins)
* [`oclif-demo plugins add PLUGIN`](#oclif-demo-plugins-add-plugin)
* [`oclif-demo plugins:inspect PLUGIN...`](#oclif-demo-pluginsinspect-plugin)
* [`oclif-demo plugins install PLUGIN`](#oclif-demo-plugins-install-plugin)
* [`oclif-demo plugins link PATH`](#oclif-demo-plugins-link-path)
* [`oclif-demo plugins remove [PLUGIN]`](#oclif-demo-plugins-remove-plugin)
* [`oclif-demo plugins reset`](#oclif-demo-plugins-reset)
* [`oclif-demo plugins uninstall [PLUGIN]`](#oclif-demo-plugins-uninstall-plugin)
* [`oclif-demo plugins unlink [PLUGIN]`](#oclif-demo-plugins-unlink-plugin)
* [`oclif-demo plugins update`](#oclif-demo-plugins-update)

## `oclif-demo hello PERSON`

Say hello

```
USAGE
  $ oclif-demo hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oclif-demo hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [src/commands/hello/index.ts](https://github.com/edezekiel/oclif-demo/blob/v0.0.0/src/commands/hello/index.ts)_

## `oclif-demo hello world`

Say hello world

```
USAGE
  $ oclif-demo hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ oclif-demo hello world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [src/commands/hello/world.ts](https://github.com/edezekiel/oclif-demo/blob/v0.0.0/src/commands/hello/world.ts)_

## `oclif-demo help [COMMAND]`

Display help for oclif-demo.

```
USAGE
  $ oclif-demo help [COMMAND...] [-n]

ARGUMENTS
  COMMAND...  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for oclif-demo.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v6.2.27/src/commands/help.ts)_

## `oclif-demo plugins`

List installed plugins.

```
USAGE
  $ oclif-demo plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ oclif-demo plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.36/src/commands/plugins/index.ts)_

## `oclif-demo plugins add PLUGIN`

Installs a plugin into oclif-demo.

```
USAGE
  $ oclif-demo plugins add PLUGIN... [--json] [-f] [-h] [-s | -v]

ARGUMENTS
  PLUGIN...  Plugin to install.

FLAGS
  -f, --force    Force npm to fetch remote resources even if a local copy exists on disk.
  -h, --help     Show CLI help.
  -s, --silent   Silences npm output.
  -v, --verbose  Show verbose npm output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into oclif-demo.

  Uses npm to install plugins.

  Installation of a user-installed plugin will override a core plugin.

  Use the OCLIF_DEMO_NPM_LOG_LEVEL environment variable to set the npm loglevel.
  Use the OCLIF_DEMO_NPM_REGISTRY environment variable to set the npm registry.

ALIASES
  $ oclif-demo plugins add

EXAMPLES
  Install a plugin from npm registry.

    $ oclif-demo plugins add myplugin

  Install a plugin from a github url.

    $ oclif-demo plugins add https://github.com/someuser/someplugin

  Install a plugin from a github slug.

    $ oclif-demo plugins add someuser/someplugin
```

## `oclif-demo plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ oclif-demo plugins inspect PLUGIN...

ARGUMENTS
  PLUGIN...  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ oclif-demo plugins inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.36/src/commands/plugins/inspect.ts)_

## `oclif-demo plugins install PLUGIN`

Installs a plugin into oclif-demo.

```
USAGE
  $ oclif-demo plugins install PLUGIN... [--json] [-f] [-h] [-s | -v]

ARGUMENTS
  PLUGIN...  Plugin to install.

FLAGS
  -f, --force    Force npm to fetch remote resources even if a local copy exists on disk.
  -h, --help     Show CLI help.
  -s, --silent   Silences npm output.
  -v, --verbose  Show verbose npm output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into oclif-demo.

  Uses npm to install plugins.

  Installation of a user-installed plugin will override a core plugin.

  Use the OCLIF_DEMO_NPM_LOG_LEVEL environment variable to set the npm loglevel.
  Use the OCLIF_DEMO_NPM_REGISTRY environment variable to set the npm registry.

ALIASES
  $ oclif-demo plugins add

EXAMPLES
  Install a plugin from npm registry.

    $ oclif-demo plugins install myplugin

  Install a plugin from a github url.

    $ oclif-demo plugins install https://github.com/someuser/someplugin

  Install a plugin from a github slug.

    $ oclif-demo plugins install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.36/src/commands/plugins/install.ts)_

## `oclif-demo plugins link PATH`

Links a plugin into the CLI for development.

```
USAGE
  $ oclif-demo plugins link PATH [-h] [--install] [-v]

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help          Show CLI help.
  -v, --verbose
      --[no-]install  Install dependencies after linking the plugin.

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ oclif-demo plugins link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.36/src/commands/plugins/link.ts)_

## `oclif-demo plugins remove [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ oclif-demo plugins remove [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ oclif-demo plugins unlink
  $ oclif-demo plugins remove

EXAMPLES
  $ oclif-demo plugins remove myplugin
```

## `oclif-demo plugins reset`

Remove all user-installed and linked plugins.

```
USAGE
  $ oclif-demo plugins reset [--hard] [--reinstall]

FLAGS
  --hard       Delete node_modules and package manager related files in addition to uninstalling plugins.
  --reinstall  Reinstall all plugins after uninstalling.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.36/src/commands/plugins/reset.ts)_

## `oclif-demo plugins uninstall [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ oclif-demo plugins uninstall [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ oclif-demo plugins unlink
  $ oclif-demo plugins remove

EXAMPLES
  $ oclif-demo plugins uninstall myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.36/src/commands/plugins/uninstall.ts)_

## `oclif-demo plugins unlink [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ oclif-demo plugins unlink [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ oclif-demo plugins unlink
  $ oclif-demo plugins remove

EXAMPLES
  $ oclif-demo plugins unlink myplugin
```

## `oclif-demo plugins update`

Update installed plugins.

```
USAGE
  $ oclif-demo plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.36/src/commands/plugins/update.ts)_
<!-- commandsstop -->
