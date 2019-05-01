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

### 6. Package Number Syntax in package.json (Symantic versioning - npm)
14.6.3 = Major release.Minor release.Patch release - Always install 14.6.3 exactly - no different version
On npm install
Caret: ^14.6.3 = ^14.x.x = Install All minor releases and patches only - Strictly Never goes to 15.0.0 - If available it will install 14.7.0 or 14.6.4 but never 15.0.0
Tilda: ~14.6.3 = ~14.6.x = Install latest patches only - Strictyl never goes to 14.7 - If available it will install 14.6.4 but never 14.7

### 7. Package.lock.json
Helps us do the same install everytime we pass our project to a different person while using ~ or ^
e.g. ^14.6.3 - Latest Install without package.lock.json might install a new ^14.25.0 which might not be the same environment the main developer was using. So, package.lock.json makes sure that same version is installed as original. Thus saving us from code breakage. Since packages are interdependent.

