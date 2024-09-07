# Test React with Github Pages

- URL : https://{ACCOUNT}.github.io/{REPO_NAME}
```shell
npx create-react-app {path} [--template typescript]
cd {path}
npm install gh-pages --save-dev
```
- edit package.json
```json
"homepage": "htpps://{ACCOUNT}.github.io/{REPO_NAME}",
"scripts": {
  ...
  "predeploy": "yarn build",
  "deploy": "gh-pages -d build"
}
```
- deploy gh-pages
```shell
yarn deploy
```
- github setting
  - repository settings > pages > branch
    - gh-pages and root

# SCSS

- need python module distutils
```shell
brew install python-setuptools
# or
python3 -m pip install setuptools
```

- install node module
```shell
yarn add node-sass
```

- rename css file to scss
```shell
mv index.css index.scss
mv App.css App.scss
```
