# Instructions

`npm init`

`npm i express`

`npm i -D typescript ts-node nodemon @types/node @types/express prettier jest`

`tsc --init`

`node -e "require('fs').writeFileSync('tsconfig.json',JSON.stringify({compilerOptions:{target:'es2016',module:'commonjs',rootDir:'./src',moduleResolution:'node',outDir:'./dist',esModuleInterop:true,forceConsistentCasingInFileNames:true,strict:true,skipLibCheck: true}}))"`

`node -e "require('fs').writeFileSync('./package.json',JSON.stringify({...require('./package.json'),scripts:{start:'node ./dist/app.js',dev:'nodemon ./src/app.t',build:'tsc -p .',test:'jest'}}));"`

`npx eslint --init`

`node -e "require('fs').writeFileSync('./.prettierrc.json',JSON.stringify({endOfLine:'auto'}));"`

`npx prettier --write .`

`node -e "require('https').get('https://raw.githubusercontent.com/github/gitignore/main/Node.gitignore',t=>{let i=require('fs').createWriteStream('./.gitignore');t.pipe(i),i.on('finish',()=>{i.close()})});"`


# with yarn

```bash
yarn init -y

yarn add express

yarn add -D typescript ts-node nodemon @types/node @types/express prettier jest eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser

node -e "require('fs').writeFileSync('./tsconfig.json',JSON.stringify({compilerOptions:{target:'es2016',module:'commonjs',rootDir:'./src',moduleResolution:'node',outDir:'./dist',esModuleInterop:true,forceConsistentCasingInFileNames:true,strict:true,skipLibCheck: true}}))"

node -e "require('fs').writeFileSync('./package.json',JSON.stringify({...require('./package.json'),scripts:{start:'node ./dist/app.js',dev:'nodemon ./src/app.t',build:'tsc -p .',test:'jest'}}));"

node -e "require('fs').writeFileSync('./.eslintrc.json',JSON.stringify({env:{browser:true,es2021:true},extends:['eslint:recommended','plugin:@typescript-eslint/recommended'],parser:'@typescript-eslint/parser',parserOptions:{ecmaVersion:'latest',sourceType:'module'},plugins:['@typescript-eslint'],rules:{}}))"

node -e "require('fs').writeFileSync('./.prettierrc.json',JSON.stringify({endOfLine:'auto'}));"

node -e "require('https').get('https://raw.githubusercontent.com/github/gitignore/main/Node.gitignore',t=>{let i=require('fs').createWriteStream('./.gitignore');t.pipe(i),i.on('finish',()=>{i.close()})});"

yarn prettier --write .
```
