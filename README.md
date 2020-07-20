# livetype
Typescript schema validation at runtime.

```ts
import typecheck from 'livetype';

const todo = await getDataFromMyServer();

if (!typecheck(todo)) {
  throw new Error('Invalid response');
}
```
And that's it. The `typecheck` function to make sure that your objects are what you think they are.

## Installation
```
npm i --save livetype
```
livetype uses source maps to reconstruct the types of your objects at runtime. Make sure that your `tsconfig.json` has the key `sourceMap` set to `true` in `compilerOptions`. Don't worry we'll yell at you if you don't have this option set!
```json
{
  "compilerOptions": {
    "sourceMap": true,
  }
}
```

## Issue Policy
Right now this repository only accepts issues from contributors. If you would like your issue to be addressed by the people working on livetype, you will have to push a commit to this repository or provide photo evidence of a financial contribution (of any amount) to one of the following organizations:
* [Black Lives Matter](https://blacklivesmatter.com/)
* [Boys and Girls Clubs of Washington](https://interland3.donorperfect.net/weblink/weblink.aspx?name=E2846&id=26)
If there are organizations you think should be added to this list please submit a PR!
