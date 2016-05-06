[![Build Status][travis-badge]][travis-link]
[![Slack Room][slack-badge]][slack-link]

# fishkit

Create a plugin from a template.

## Install

With [fisherman]

```
fisher fishkit
```

## Usage

```
fishkit [TEMPLATE]
```

Or with a [strings](#strings) file.

```
fishkit TEMPLATE < strings.yaml
```


## Example

```
fishkit plugin
```
```
❯ What's your plugin name? tron
❯ What's your plugin about? It's just pong
❯ What's your GitHub username? flynn
    .editorconfig
    .gitignore
    .travis.yml
    completions/tron.fish
    functions/tron.fish
    LICENSE
    README.md
```

## Strings

```
fishkit TEMPLATE < strings.yml
```

```yml
name: tron
description: It's just pong
author: Kevin Flynn
owner: flynn
```

## Templates

The available templates are:

* [Plugin]
* [Prompt]
* [Snippet]


[fisherman]: https://github.com/fisherman/fisherman

[slack-link]: https://fisherman-wharf.herokuapp.com
[slack-badge]: https://fisherman-wharf.herokuapp.com/badge.svg
[travis-link]: https://travis-ci.org/fisherman/fishkit
[travis-badge]: https://img.shields.io/travis/fisherman/fishkit.svg

[Plugin]: https://github.com/fisherman/fishkit/tree/master/templates/plugin
[Prompt]: https://github.com/fisherman/fishkit/tree/master/templates/prompt
[Snippet]: https://github.com/fisherman/fishkit/tree/master/templates/snippet
