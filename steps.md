## Steps to create a base project

1.  Initialize npm: npm init
2.  initialize repository on git:
    - git init
    - git add .
    - commit -m "added initial files to project"
    - go to git and create a new repository
    - rename git branch from master to main: git branch -M main
    - add git remote: git remote add origin (copy from git repo)
    - set up upstream and push: git push -u origin maingit push -u origin main
3.  create a folder:
    - public
      - temp
        - .gitkeep
    - src
      - controllers (folder)
      - db (folder)
      - middlewares (folder)
      - models (folder)
      - routes (folder)
      - utils (folder)
      - app.js (file)
      - constants.js (file)
      - index.js (file)
4.  create files:
    - .gitignore (the sensetive files which will be excluded from git push)
    - google git ignore generator and enter node as eniviroment. It will give us all the things to put into the .gitignore file
5.  create an enviroment variable file: .env
6.  Install nodemon: npm i -D nodemon
    - inside package.json type "dev": "nodemon src/index.js" under the scripts
7.  Install prettier: npm i -D prettier - in root folder, create a file: .prettierrc. Inside prettier:

```javascript
    {
    "singleQuote": false,
    "bracketSpacing": true,
    "tabWidth": 2,
    "trailingComma": "es5",
    "semi": true
    }
```

8. In root create a file .prettierignore. Inside:

```javascript
/.vscode
/node_modules
./dist
*.env
.env
.env.*
```

8.  in package.json, add:
    - "type": "module"
