# Node Package Manager
## Introduction
In this repository you'll find my personal practice for the course Dependencies and Packages Management in [Platzi](https://platzi.com/clases/npm).

## Table of contents
* [General info](#general-info)
* [Setup](#Setup)
* [The Swiss Army Knife for NPM](#the-swiss-army-kife)

## General Info
During the course, we've learned the basics about [Node Package Management](https://docs.npmjs.com/about-npm), the open source package manager for the Node.JS platform. The goal of the code you'll find in this repo was to create my first own package for NPM.
If anyone feels like adding or improving something, feel free to do so!

## Setup
In order to get install the dependencies found in package.json you need to run the command `npm install`.
After you've done that, you can simply run the following command in your bash:

```
npm link
```

and to see what's been done, you only need to run `random`. 

**Have fun!**

## The Swiss Army Knife

```
npm init [--yes|-y|--scope]
```

\* It can be used to set up a new or existing npm package.

```
npm install (with no args, in package dir)

aliases: npm i, npm add
common options: [--save|-D|--save-dev|-O|--save-optional] [-E|--save-exact] [-g|--global] [--no-save] [--dry-run]
```

\* This command installs a package and any packages that it depends on.

```
npm audit

npm audit fix
```

\* It submits a description of the dependencies configured in your project to your default registry and asks for a report of known vulnerabilities. If the fix argument is provided, then remediations will be applied to the package tree.

```
npm run <script>
```

\* This runs an arbitrary command from a package's scripts object. If no command is provided, it will list the available scripts.

```
npm link (in package dir)

alias: npm ln
```

\* This is handy for installing your own stuff, so that you can work on it and test iteratively without having to continually rebuild.

```
npm publish [<tarball>|<folder>] [--tag <tag>] [--access <public|restricted>] [--otp otpcode] [--dry-run]
```

\* It publishes a package to the registry so that it can be installed by name.

```
npm outdated [[<@scope>/] <pkg> ...]
```

\* This command will check the registry to see if any (or, specific) installed packages are currently outdated.

```
npm update [-g] [<pkg>...]

aliases: up, upgrade
```

This command will update all the packages listed to the latest version (specified by the tag config), respecting semver.

```
npm config set <key>=<value> [<key>=<value> ...]
npm config get [<key> [<key> ...]]
npm config delete <key> [<key> ...]
npm config list [--json]
npm config edit
npm set <key>=<value> [<key>=<value> ...]
npm get [<key> [<key> ...]]

alias: c
```

\* npm gets its config settings from the command line, environment variables, npmrc files, and in some cases, the package.json file. It can be used to update and edit the contents of the user and global npmrc files.

```
npm help <term> [<terms..>]
```

\* If supplied a topic, then show the appropriate documentation page.






 

