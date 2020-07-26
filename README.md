## Hyperapp + Jest

This project is used as a case-study to illustrate an issue when running Jest tests with Hyperapp.

Follow the steps below to reproduce the issue.

Install dependencies:
```
npm install
or
yarn install
```

Run the tests:
```
npm run test
or
yarn test
```

Notice that the failed test `index2.spec.js` uses an `import` but so does the `index.spec.js` (which passes).

This illustrates the fact that in order to import `Hyperapp` in **Jest tests**, some extra configuration might be necessary.
