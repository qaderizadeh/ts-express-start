# Instructions

`npm init`

`npm i express`

`npm i -D typescript ts-node nodemon @types/node @types/express prettier jest`

`tsc --init`

edit `tsconfig.json`

  `{
  "compilerOptions": {
    "target": "es2016",
    "module": "commonjs",
    "rootDir": "./src",
    "moduleResolution": "node",
    "outDir": "./dist",
    "esModuleInterop": true,
    "forceConsistentCasingInFileNames": true,
    "strict": true,
    "skipLibCheck": true
  }
}`
  


edit `package.json`

  `"scripts": {
    "start": "node ./dist/app.js",
    "dev": "nodemon ./src/app.t",
    "build": "tsc -p .",
    "test": "jest"
  }`
  

`npx eslint --init`

`echo { "endOfLine": "auto" } > .prettierrc.json`

https://github.com/github/gitignore/raw/main/Node.gitignore
