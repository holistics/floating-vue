# `@holistics/floating-vue`

## About the fork

This fork has the `@holistics/floating-vue` package that tries to fix the following issues:

- **[Performance]** Disable toggling CSS class of `<body>`: this makes the entire page reflow whenever some floating elements are shown/all are hidden ([PR #1019](https://github.com/Akryum/floating-vue/pull/1019)). Can be re-enabled via `toggleBodyClass` prop.
- **[Fix]** Properly fix diagonal submenu problem ([#916](https://github.com/Akryum/floating-vue/issues/916)) via `fixDiagonalSubmenuProblem` prop
- **[Fix]** Fix sibling submenus not showing after current submenu is timed out and hidden

### 📦️ Versioning and syncing

> This fork uses `<pre-release>` verison under the identifier `holistics` to preserve changes between forked versions. For example, `5.2.2-holistics.1` means:
>
> - `5.2.2` is the version that was forked
> - `holistics` is the `<pre-release identifier>`
> - `1` is the first change to the version forked above (ranges from [0..+infinity])

To sync with the latest version of the original package (e.g. version `5.9.0`):

1. Use `git merge upstream/main --no-commit` and resolve conflicts if have any
2. Bump to the latest version in [`packages/floating-vue/package.json`](./packages/floating-vue/package.json) (e.g. `5.9.0-holistics.0`)
3. Add a new [CHANGELOG](./CHANGELOG.md) entry
4. Commit the changes
5. Publish the package to both Holistics internal and NPM registries (must use `npm`):

    ```sh
    $ cd packages/floating-vue
    $ npm publish
    # NPM registry
    $ npm publish --access=public --@holistics:registry=https://registry.npmjs.org/
    ```

<p align="center">
<img src="./logo.png" alt="Floating Vue logo"/>
</p>

<h1 align="center">Floating Vue</h1>

<p align="center">
<a href="https://www.npmjs.com/package/floating-vue"><img src="https://img.shields.io/npm/v/floating-vue.svg"/> <img src="https://img.shields.io/npm/dm/floating-vue.svg"/></a> <a href="https://vuejs.org/"><img src="https://img.shields.io/badge/vue-3|2-brightgreen.svg"/></a>
</p>

<p align="center">
Easy tooltips, dropdowns, menus... with <a href="https://github.com/floating-ui/floating-ui">Floating UI</a>
</p>

<p align="center">
  <a href="https://floating-vue.starpad.dev/"><b>📚️ Documentation</b></a>
</p>

The package has been renamed from `v-tooltip` to `floating-vue` and now uses [floating-ui](https://floating-ui.com) instead of popperjs. You can find the new changelog for both v1 (for Vue 2) and v2 (for Vue 3) [here](https://github.com/Akryum/floating-vue/blob/main/CHANGELOG.md). The changelog is currently not pushed to GitHub Releases.

New versions:

|Old|New|Target
|---|---|---|
|v-tooltip v3|floating-vue v1|Vue 2|
|v-tooltip v4|floating-vue v5|Vue 3|

[💚️ Become a Sponsor](https://github.com/sponsors/Akryum)

## Sponsors

<p align="center">
  <a href="https://guillaume-chau.info/sponsors/" target="_blank">
    <img src='https://akryum.netlify.app/sponsors.svg'/>
  </a>
</p>

---

LICENCE MIT - Created by Guillaume CHAU (@Akryum)
