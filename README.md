# docusaurus-lunr-search
Offline Search for Docusaurus V2

[Demo Website](https://lelouch77.github.io/docusaurus-lunr-search-demo/)

 [![MIT Licence](https://img.shields.io/github/license/lelouch77/docusaurus-lunr-search)](#)

[![npm version](https://badge.fury.io/js/docusaurus-lunr-search.svg)](https://www.npmjs.com/package/docusaurus-lunr-search)

## Sample
<p align="center">
  <img width="460" height="300" src="https://raw.githubusercontent.com/lelouch77/docusaurus-lunr-search/master/assets/search-offline.png">
</p>

## How to Use ?
1. Install this package
```
npm i docusaurus-lunr-search  --save

```
2. Then run docusaurus swizzle
```
npm run swizzle docusaurus-lunr-search SearchBar
```
3. Add the docusaurus-lunr-search plugin to your `docusaurus.config.js`
```
const path = require('path');
module.exports = {
  // ...
    plugins: [path.resolve(__dirname, './node_modules/docusaurus-lunr-search/')],
}
```
4. Then build your Docusaurus project
```
npm run build
```
5. Serve your application
```
npx http-server ./build
```

Note: Docusaurus search information can only be generated from a production build. Local development is currently not supported.

## Language options
```
const path = require('path');
module.exports = {
  // ...
    plugins: [[ path.resolve(__dirname, './node_modules/docusaurus-lunr-search/'), {
      languages:['en', 'de'] // language codes
    }],
}
```
Supports all the language listed here https://github.com/MihaiValentin/lunr-languages


Thanks to [`algolia/docsearch.js`](https://github.com/algolia/docsearch), I modified it to create this search component 
