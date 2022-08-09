# npm-copy-test

This repo demonstrates how to use the [npm copy](https://github.com/npm/cli/pull/4082) command to deploy single apps from a monorepo.

## Demo

```bash
# pull the repo, then:
npm install
cd packages/app
npx npm copy .deploy # runs local npm
# files are bundled to packages/app/.deploy directory
```

## How to use

1. Install npm dev branch locally:
```json
{
  "devDependencies": {
    "npm": "everett1992/cli#copy"
  }
}
```

2. Use npx to run the copy command from within the project:
```bash
npx npm copy .deploy
```
