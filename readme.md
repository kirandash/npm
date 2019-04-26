## npm

### 1. Creating a package
npm.init
package.json

### 2. Installing dependencies and dev dependencies
Dependencies: Packages that we need in both development and production. Will be included in production build.
npm install bootstrap
or 
npm install express
Dev dependencies: Packages that we need only during development. Will not be included in production build.
npm install babel-cli babel-preset-stage-0 babel-preset-es2015 --save-dev