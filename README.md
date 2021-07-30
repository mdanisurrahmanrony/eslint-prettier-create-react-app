#### 1. Create React App

```
npx create-react-app eslint-prettier-create-react-app
```

#### 2. Install `Visual Studio Code` plugins

```
ESLint by Dirk Baeumer, Prettier - Code formatter by Prettier, Dracula Official Theme (optional)
```

#### 3. Install dev dependencies

```
yarn add prettier eslint-config-prettier eslint-plugin-prettier -D
```

#### 4. Create `.eslintrc` file in the project root and enter the below contents:

```
{
    "extends": ["react-app", "plugin:prettier/recommended"],
    "rules": {
        "prettier/prettier": [
          "error",
          {
            "singleQuote": true
          }
        ]
      }
}
```

#### 5. Follow the below settings for `User Settings` of `Visual Studio Code`

```
{
    "editor.formatOnSave": true,
    "[javascript]": {
        "editor.formatOnSave": false
    },
    "eslint.alwaysShowStatus": true,
    "files.autoSave": "onFocusChange",
    "workbench.colorTheme": "Dracula"
}
```

#### 6. Install `husky lint-staged` dev dependency

```
yarn add husky lint-staged -D
```

#### 7. Install `pretty-quick` dev dependency

```
yarn add pretty-quick -D
```

#### 8. Add `precommit` scripts inside `package.json` file

```
  "scripts": {
    "precommit": "pretty-quick --staged"
  }
```

#### 9. References

```
https://www.youtube.com/watch?v=bfyI9yl3qfE
```
