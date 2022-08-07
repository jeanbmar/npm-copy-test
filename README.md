# npm-copy-test

This repo demonstrates how to use the [npm copy](https://github.com/npm/cli/pull/4082) command to deploy single apps from a monorepo.

## Demo

```bash
# pull the repo, then:
npm install
cp packages/app
npm run copy # this wraps the npm copy from the dev branch since it's not available on npm yet
# files are bundled to packages/app/.deploy directory
```
