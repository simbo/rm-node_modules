rm-node_modules
===============

> A shell script to find and delete all node_modules directories recursively
> within a given path.

[![GitHub Release](https://img.shields.io/github/v/release/simbo/rm-node_modules)](https://github.com/simbo/rm-node_modules/releases)
[![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/simbo/rm-node_modules/CI/master)](https://github.com/simbo/rm-node_modules/actions?query=workflow%3ACI)
![Pure Bash Script](https://img.shields.io/badge/pure-bash-green)


---

## About

Working with node.js projects for some time, your disk space will be filled with
`node_modules` directories taking up quite some space. This script finds them,
lists them and deletes them in a quick and convenient way, while optionally
determining the disk usage of respective directories.

## Requirements

This script should work with every linux or mac platform where bash is available.  
(bash doesn't need to be your default shell.)

If you experience any problems, please [create an issue](https://github.com/simbo/rm-node_modules/issues).

## Install and Update

To install and/or update, simply run the following command:

```sh
curl -so- https://raw.githubusercontent.com/simbo/rm-node_modules/master/install | bash
```

This will install `rm-node_modules` to `$HOME/bin`.

Afterwards, you can run the script using `rm-node_modules` or `rmnm`.

### Installing manually

Download [./rm-node_modules](https://raw.githubusercontent.com/simbo/rm-node_modules/master/rm-node_modules)
and put it anywhere you want.

Make sure, it's within your `$PATH`.

Make it executable: `chmod +x ./rm-node_modules`

And optionally link it with a short alias: `ln -s ./rm-node_modules rmnm`

## Usage

```sh
Usage:  rmnm [-yuv] [-d <DIR>]

Options:
  -d <DIR>  directory to search within (default: current directory)
  -y        delete without confirmation
  -u        determine disk usage
  -v        display version info only
```

## Screenshots

### Default Output

![rm-node_modules default output](./screenshot-default.png)

### Output with Disk Usage

![rm-node_modules with disk usage](./screenshot-disk-usage.png)

## License and Author

[MIT &copy; Simon Lepel](http://simbo.mit-license.org/)
