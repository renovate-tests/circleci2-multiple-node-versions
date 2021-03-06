circleci2-multiple-node-versions
====
Sample project to build with multiple Node.js versions in CircleCI 2.0!

[![build status][circleci-image]][circleci-url]
![Node.js Version Support][node-version]

## Branches

- [yarn](https://github.com/teppeis-sandbox/circleci2-multiple-node-versions/tree/yarn) (master)
- [yarn-with-test-report](https://github.com/teppeis-sandbox/circleci2-multiple-node-versions/tree/yarn-with-test-report)
- [npm](https://github.com/teppeis-sandbox/circleci2-multiple-node-versions/tree/npm)
- [npm-with-test-report](https://github.com/teppeis-sandbox/circleci2-multiple-node-versions/tree/npm-with-test-report)

Note: `npm` and `npm-with-test-report` uses `package-lock.json` introduced by npm@5.
So the lock file is ignored in npm@2, 3 and 4 (and Node v4 and v6 bundle npm@2 and 3 respectively).

## How to use

1. Copy `.circleci/config.yml` to your project
2. [Add your project to CircleCI](https://circleci.com/docs/2.0/first-steps/)
3. Open your project settings in CircleCI 2.0 and add a new "Environment Variables"
  - name: `CIRCLE_CACHE_VERSION`, value: 1
4. Rebuild

## License

MIT License: Teppei Sato &lt;teppeis@gmail.com&gt;

[circleci-image]: https://circleci.com/gh/teppeis-sandbox/circleci2-multiple-node-versions.svg?style=shield
[circleci-url]: https://circleci.com/gh/teppeis-sandbox/circleci2-multiple-node-versions
[node-version]: https://img.shields.io/badge/Node.js%20support-v4,v6,v8-brightgreen.svg
