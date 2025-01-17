# @commercetools-frontend/codemod

<p align="center">
  <a href="https://www.npmjs.com/package/@commercetools-frontend/codemod"><img src="https://badgen.net/npm/v/@commercetools-frontend/codemod" alt="Latest release (latest dist-tag)" /></a> <a href="https://www.npmjs.com/package/@commercetools-frontend/codemod"><img src="https://badgen.net/npm/v/@commercetools-frontend/codemod/next" alt="Latest release (next dist-tag)" /></a> <a href="https://bundlephobia.com/result?p=@commercetools-frontend/codemod"><img src="https://badgen.net/bundlephobia/minzip/@commercetools-frontend/codemod" alt="Minified + GZipped size" /></a> <a href="https://github.com/commercetools/merchant-center-application-kit/blob/main/LICENSE"><img src="https://badgen.net/github/license/commercetools/merchant-center-application-kit" alt="GitHub license" /></a>
</p>

Codemod transformations for Custom Applications.

## Usage

```bash
$ npx @commercetools-frontend/codemod@latest <transform> <glob_pattern>
```

We recommend to run `prettier` on the modified files to preserve the formatting configured on your project. For example, you can run `prettier --write $(git diff --name-only)`.

> If you are using `lint-staged` there is a high chance that you already run `prettier` on the staged files. Therefore, you don't need to run it manually.

## Transforms

### `remove-deprecated-modal-level-props`

Remove deprecated `level` and `baseZIndex` props from modal page components.

```
$ npx @commercetools-frontend/codemod@latest remove-deprecated-modal-level-props 'src/**/*.{js,jsx,ts,tsx}'
```

### `rename-js-to-jsx`

Rename `.js` files using React JSX syntax to `.jsx`.

```
$ npx @commercetools-frontend/codemod@latest rename-js-to-jsx 'src/**/*.js'
```

### `rename-mod-css-to-module-css`

Rename `.mod.css` files to `.module.css` and update imports.

```
$ npx @commercetools-frontend/codemod@latest rename-mod-css-to-module-css 'src/**/*.{js,jsx,ts,tsx}'
```
