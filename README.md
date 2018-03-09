# Angular 2 Wallaby Demo
Set up Wallaby for Angular. This guide assumes you have Wallaby.js extension installed for VS Code and Angular CLI installed globally.

1. Create angular cli project
```
ng new PROJECT-NAME
cd PROJECT-NAME
ng serve
````

2. Add the wallaby.js config file to the project.
`https://github.com/wallabyjs/ngCliWebpackSample/blob/master/wallaby.js`


3. Add wallaby.js test bootstrap to src folder
`https://github.com/wallabyjs/ngCliWebpackSample/blob/master/src/wallabyTest.ts`

4. Exclude the `src/wallabyTest.ts` file in the tsconfig.json as it may affect Angular AOT compilation.

4. Install dependencies
`npm install wallaby-webpack angular2-template-loader electron --save-dev`

5. Select config file (wallaby.js) by typing `Wallaby.js: Select Configuration File` in the command pallete

6. Start Wallaby.js by running `Wallaby.js: Start` in the command pallete
