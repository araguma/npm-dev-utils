# npm-dev-utils

npm-dev-utils is a collection of cross-platform compatible functions and shell commands that aid in npm package development. It includes commonly used commands like `rm -rf` for removing build directories or `concurrent` for running multiple commands at the same time. There is also the `server` command which hosts a locally static server for developing websites. For more available commands, please see the command section below.

## Installation

### Latest version
```bash
npm i -D https://github.com/araguma/npm-dev-utils.git#latest
```

### Latest stable version
```bash
npm i -D https://github.com/araguma/npm-dev-utils.git
```

## Commands

```
Usage: du [options] [command]

A collection of cross-platform compatible functions and shell commands that aid in npm package development

Options:
  -V, --version                      output the version number
  -h, --help                         display help for command

Commands:
  concurrent <string...>             Run multiple commands concurrently
  cp [options] <string> <string>     Copy path contents to another destination
  mkdir [options] <string>           Create a directory
  rm [options] <string>              Remove path
  server [options] <string>          Start a static local server
  watch [options] <string> <string>  Watch a path for changes
  help [command]                     display help for command
```

## Examples

Removing a directory
``` bash
npx du rm -rf directory/to/remove/
```

Hosting a local server
``` bash
npx du server -p 3000 server/root/directory/
```
