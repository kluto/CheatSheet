
### VUE Development
#### Extensions
- Vetur
- ESLint
- Prettier

Vetur comes with its own linting features. But to avoid syntax checking conflict with ESLint, we should turn off Vetur’s template validation. Go to Code > Preferences > Settings, and then search vetur.validation.template. You should see a checkbox for disabling Vetur’s template validation. Uncheck the box to turn off Vetur’s template checking.

npm install --save-dev @vue/eslint-config-prettier prettier eslint-plugin-prettier

#### Files
Create .prettierrc.js:
```
module.exports = {
    singleQuote: true,
    semi: false
}
```
Create .jsconfig.json:
```
{
    "include": [
        "./src/**/*"
    ]
}
```
Add to .eslintrc.js:
```
...
"extends":
  ...
  "@vue/prettier"
  ...
],
...
```
Add to settings.json:
```
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    }
```

### Themes
- Dark: Monokai Dimmed
- Light: Winter is Coming
