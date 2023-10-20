# Overview

Sometimes you will want to create a `npm package` there are several reasons to do this, you want to share code between services, the code is very large to have them in one repo or want to create a custom framework, whatever the reason this is the guide and steps to achieve this.

# Instructions

1. Go to [npm page](https://www.npmjs.com/)
2. click on the profile menu and `create organization`
3. choose a name and select the `free option`
4. If you want you can invite devs

Great! now you have a brand new organization created, now comes the funny part create and configure the folder/project to achieve this

5. Create a new folder the usual name for this types of package is `common` but you can choose the name you want (be creative)
   ```console
   mkdir common
   cd common/
   ```
6. Open your `package.json` and change the name for the organization name you created on npm webpage + the name of the project, like this

   ```json
   {
     "name": "@kytickets/common",
     "version": "1.0.0",
     "description": "",
     "main": "./build/index.js",
     "types": "./build/index.d.ts",
     "file": ["build/**/*"],
     "scripts": {
       "clean": "del ./build/*",
       "build": "npm run clean && tsc",
       "pub": "git add . && git commit -m \"Updates\" && npm version patch && npm run build && npm publish && git push"
     },
     "keywords": [],
     "author": "",
     "license": "ISC",
     "devDependencies": {
       "@types/typescript": "^2.0.0",
       "del-cli": "^5.0.0",
       "typescript": "^4.9.4"
     }
   }
   ```

7. Initialize `git` link to a repo, add the changes and push

   ```console
   git init
   git remote add origin <gh link>
   git add .
   git commit -m "First commit"
   git push
   ```

8. Login to `npm`

   ```console
   npm login
   ```

9. Publish you module for the first time

   ```console
   npm publish --access public
   ```

10. When you do a change you can publish it with

    ```console
    npm run pub
    ```

# Install and use this in project

So now we're ready with our package published and ready to use, the only thing left is to install it on the project

```console
npm install @kytickets/common
```

# Update the package in you project

So when you push a new version of your package you will want the latest changes in you target project

```console
npm update @kytickets/common
```
