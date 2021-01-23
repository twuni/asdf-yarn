# asdf-yarn

[![Build Status][3]][4]

Yarn plugin for the [asdf][1] version manager.

> 💡 **Note:** This plugin validates package authenticity via [`gpg`][2].

## Requirements

This plugin should work out of the box on Linux and Mac operating systems.
If one of the commands needed is unavailable, it will let you know.

## Installing

```
asdf plugin-add yarn
asdf install yarn latest
```

## Looking for Yarn v2?

In v2.x, Yarn introduced its own version manager which can only be
configured on a per-project basis. There is no "global install" variation
of the v2.x release line.

To use Yarn v2.x in your project:

 1. Use this plugin to set the v1.x Yarn version for the project
    (e.g: `asdf local yarn 1.22.10`).

 2. Use Yarn to set the v2.x Yarn version for the project
    (e.g: `yarn set version 2.4.1`).

After these two steps, your project will be configured to use Yarn v2.x.
If you do not wish to opt in to v2.x, then step 1 is all you need.

[1]: https://asdf-vm.com/
[2]: https://www.openpgp.org/
[3]: https://travis-ci.org/twuni/asdf-yarn.svg?branch=master
[4]: https://travis-ci.org/twuni/asdf-yarn
