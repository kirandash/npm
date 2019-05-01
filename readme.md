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

### 3. Installing a package globally
npm install -g @angular/cli
or 
npm install -g react
or
npm install -g react-tools

### 4. Updating a package
npm install bootstrap@3
To check what are all the outdated packages in your current project: 
npm outdated
To check all outdated packages from your machine globally:
npm outdated -g
Install all the outdated packages again to update it to latest version:
npm install bootstrap
By default wanted version will be installed. Which can be changed by
npm install bootstrap@latest

Note: If any issue comes related to admin permission etc, uninstall npm and install again to latest version.

### 5. Uninstalling a package
npm uninstall babel-preset-es2015
npm install babel-preset-env --save-dev