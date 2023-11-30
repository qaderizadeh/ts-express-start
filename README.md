# Instructions

`npm init`

`npm i express`

`npm i -D typescript ts-node nodemon @types/node @types/express prettier`

`tsc --init`

edit `tsconfig.json`

  `rootDir: ./src`
  
  `outDir: ./dist`
  
  `moduleResolution: node`
  


edit `package.json`

  `start: node ./dist/app.js`
  
  `dev: nodemon src/app.ts`
  
  `build: tsc -p .`
  
  `test: jest`
  

`npx eslint --init`

`echo { "endOfLine": "auto" } > .prettierrc.json`

https://github.com/github/gitignore/raw/main/Node.gitignore
