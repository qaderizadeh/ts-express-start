# Instructions

`npm i -g typescript`
`tsc --version`
`tsc --init`

edit `tsconfig.json`
  rootDir: ./src
  outDir: ./dist
  moduleResolution: node

`npm init`
`npm i express`
`npm i -D typescript ts-node nodemon @types/node @types/express`

edit `package.json`
  start: noe ./dist/app.js
  dev: nodemon src/app.ts
  build: tsc -p .

`npx eslint --init`

`npm i -D --save-exact prettier`
`echo {}>.prettierrc.json`
