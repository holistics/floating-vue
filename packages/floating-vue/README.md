# `@holistics/floating-vue`

## About the fork

This fork has the `@holistics/floating-vue` package that tries to fix some issues of the original package.

### 📦️ Versioning and syncing

> This fork uses `<pre-release>` verison under the identifier `holistics` to preserve changes between forked versions. For example, `5.2.2-holistics.1` means:
>
> - `5.2.2` is the version that was forked
> - `holistics` is the `<pre-release identifier>`
> - `1` is the first change to the version forked above (ranges from [0..+infinity])

To sync with the latest version of the original package (e.g. version `5.9.0`):

1. Use `git merge upstream/main --no-commit` and resolve conflicts if have any
2. Bump to the latest version in [`package.json`](./package.json) (e.g. `5.9.0-holistics.0`)
3. Add a new [CHANGELOG](./CHANGELOG.md) entry
4. Commit the changes
5. Publish the package to both Holistics internal and NPM registries (must use `npm`):

    ```sh
    $ npm publish
    # NPM registry
    $ npm publish --access=public --@holistics:registry=https://registry.npmjs.org/
    ```

<p align="center">
<img src="./logo.png" alt="floating-vue logo"/>
</p>

<h1 align="center">Floating Vue</h1>

<p align="center">
<a href="https://www.npmjs.com/package/floating-vue"><img src="https://img.shields.io/npm/v/floating-vue.svg"/> <img src="https://img.shields.io/npm/dm/floating-vue.svg"/></a> <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/vue-3|2-brightgreen.svg"/></a>
</p>

<p align="center">
Easy tooltips, dropdowns, menus... with <a href="https://github.com/floating-ui/floating-ui">Floating UI</a>
</p>

<p align="center">
  <a href="https://floating-vue.starpad.dev/">Documentation</a>
</p>

[💚️ Become a Sponsor](https://github.com/sponsors/Akryum)

## Sponsors

[![sponsors logos](https://guillaume-chau.info/sponsors.png)](https://guillaume-chau.info/sponsors)

---

LICENCE MIT - Created by Guillaume CHAU (@Akryum)
