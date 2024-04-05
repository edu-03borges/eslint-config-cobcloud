# ESLint Config CRM - CobCloud

## Whats included?

- Standard config base;
- React plugin;
- React Hooks plugin;
- JSX a11y plugin;
- ESLint;
- Prettier;
- Tailwind CSS;

## Setup

## Required >= React v17.0 And >= Node Js v16.0

## Install Extension in Vscode ESLint and Uninstall Prettier

Install EsLint:
```
https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint
```

Uninstall Prettier:
```
[https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
```

## Configuration File Prettier

You can configure Prettier via (in order of precedence):
```
A "prettier" key in your package.json file.
A .prettierrc file written in JSON or YAML.
A .prettierrc.json, .prettierrc.yml, .prettierrc.yaml, or .prettierrc.json5 file.
A .prettierrc.js, or prettier.config.js file that exports an object using export default or module.exports (depends on the type value in your package.json).
A .prettierrc.mjs, or prettier.config.mjs file that exports an object using export default.
A .prettierrc.cjs, or prettier.config.cjs file that exports an object using module.exports.
A .prettierrc.toml file.
```

## Vs Code - Open User Settings (JSON)

Inside `settings.json`
```
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit",
    "source.organizeImports": "explicit"
  }
```

## Configuration `package.json`

Inside `package.json`
```
{
  "scripts": {
    "lint": "eslint . --ext .js,.jsx,.ts,.tsx --fix"
  }
}
```

### React (without Next.js): JavaScript Support

Install dependencies:
```
npm install eslint prettier prettier-plugin-tailwindcss eslint-plugin-prettier eslint-config-prettier eslint-plugin-jsx-a11y eslint-plugin-n eslint-plugin-import eslint-plugin-promise eslint-plugin-react eslint-plugin-react-hooks babel-eslint eslint-config-standard eslint-plugin-standard --save-dev
```
OR
```
yarn add eslint prettier prettier-plugin-tailwindcss eslint-plugin-prettier eslint-config-prettier eslint-plugin-jsx-a11y eslint-plugin-n eslint-plugin-import eslint-plugin-promise eslint-plugin-react eslint-plugin-react-hooks babel-eslint eslint-config-standard eslint-plugin-standard --dev
```

Inside `.eslintrc.json`
```
Copy content from reactWithoutNextJsForJavaScript.json
```

Inside `.prettierrc`
```
{
  "plugins": ["prettier-plugin-tailwindcss"]
}
```

### Node.js: JavaScript Support

Install dependencies:
```
npm install eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-n eslint-plugin-import eslint-plugin-promise babel-eslint eslint-config-standard eslint-plugin-standard --save-dev
```
OR
```
yarn add eslint prettier eslint-plugin-prettier eslint-config-prettier eslint-plugin-n eslint-plugin-import eslint-plugin-promise babel-eslint eslint-config-standard eslint-plugin-standard --dev
```

Inside `.eslintrc.json`
```
Copy content from nodeForJavaScript.json
```
