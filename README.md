# npm-copy-test

This repo demonstrates how to use the [npm copy](https://github.com/npm/cli/pull/4082) command to deploy single apps from a monorepo.

## Demo

```bash
# pull the repo, then:
npm install
cd packages/app
npm run copy # this wraps the npm copy from the dev branch since it's not available on npm yet
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

2. Use npx to run the copy command:
```json
{
  "scripts": {
    "copy": "npx npm copy .deploy"
  },
}
```
