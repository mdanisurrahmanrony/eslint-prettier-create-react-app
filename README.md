#### 1. Create React App

```
npx create-react-app eslint-prettier-create-react-app
```

#### 2. Install plugins

```
ESLint by Dirk Baeumer, Prettier - Code formatter by Prettier, Dracula Official Theme (optional)
```

#### 3. Install Dev Dependencies

```
yarn add prettier eslint-config-prettier eslint-plugin-prettier -D
```

#### 4. Create a .eslintrc file in the project root and enter the below contents:

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

#### 5. Follow the below settings for `User Settings` of VS Code

```
{
    "editor.formatOnSave": true,
    "[javascript]": {
        "editor.formatOnSave": false
    },
    "eslint.alwaysShowStatus": true,
    "files.autoSave": "onFocusChange",
}
```

#### 6. Install `husky lint-staged` Dev Dependency

```
yarn add husky lint-staged -D
```

#### 7. Install `pretty-quick` Dev Dependency

```
yarn add pretty-quick -D
```

#### 8. References

```
https://www.youtube.com/watch?v=bfyI9yl3qfE
https://www.youtube.com/watch?v=C7D4nMvbdFQ
```
