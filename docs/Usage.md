# Usage

You need to have React [`16.8.0`](https://reactjs.org/blog/2019/02/06/react-v16.8.0.html) or later installed to use the Hooks API. You can import each hook individually

```js
import useToggle from 'use-react-hook/lib/useToggle'
```

or use ES6 named imports (tree shaking recommended)

```js
import {useToggle} from 'use-react-hook'
```

Depending on your bundler you might run into a missing dependency error with ES6 named import statements. Some hooks require you to install peer dependencies so we recommend using individual imports. If you want the best of both worlds you can transform the named import statements to individual import statements with [`babel-plugin-import`](https://github.com/ant-design/babel-plugin-import) by adding the following config to your `.babelrc` file:

```json
[
      'import',
      {
        libraryName: 'use-react-hook',
        camel2DashComponentName: false,
        customName(/** @type {string} */ name) {
          const libraryDirectory = name.startsWith('Use')
            ? 'lib/component'
            : name.startsWith('create')
            ? 'lib/factory'
            : 'lib'
          return `use-react-hook/${libraryDirectory}/${name}`
        }
      },
      'import-use-react-hook'
    ]
```
