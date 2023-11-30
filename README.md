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

https://github.com/github/gitignore/raw/main/Node.gitignore
