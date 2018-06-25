# nodevl

Simple Nodejs app reloader for development.

This will reload the app when any of the files are changed, edited, deleted or saved.

#### Install
- Install as a dev-dependecy `npm i nodevl --save-dev` or `yarn add nodevl --dev`
- Install as a global module `npm i nodevl -g`

#### Usage
- As a dev-dependency On `package.json` create a script `dev: nodevl your.js` and run it with `npm run dev`
- As a global module, you can directly run `nodevl your.js` is similar to running `node your.js`

#### Environment Variables
- You can pass extra environment variables by using `--env` option. eg. `nodevl your.js --env=PORT=8080,DEBUG=*`

#### Ignoring Directories/Files
- By default, this module ignores the `node_modules` folder in addition, you can also pass `--ignored` option to add ignored directories/folders/file. eg. `nodevl your.js --ignored=dist/test,test,build` this will ignore `dist/test`, `test`, and `build` folders