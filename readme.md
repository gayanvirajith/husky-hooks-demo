# git commit hooks for jira

## Instructions

- `npm install husky --save-dev`
- `npm install --save-dev @commitlint/cli commitlint-plugin-jira-rules commitlint-config-jira`
- Create a file `commitlint.config.js` and include below statements
```javascript
module.exports = {
  plugins: ['commitlint-plugin-jira-rules'],
  extends: ['jira']
}
```
- Update `package.json` file with below contents

```json
  "husky": {
    "hooks": {
      "commit-msg": "commitlint -E HUSKY_GIT_PARAMS"
    }
  }
```

readme
1
1
1
1
1
1
1
1
1
1
