![](https://img.shields.io/badge/Microverse-blueviolet)

# Potfolio Setup and Mobile First 

> This is the first page of the Porfolio template. The design are given by the 
> Microverse that I have made it 


## Built With

- HTML, CSS
- Linters for checking error
- Technologies used



## Getting Started

This project incilude toolbar and headlines 
In other to run this you need a local copy. Fist you need to setup a Linters adn the follow the coomad and the end I will give a 
screenshot that there is no error in linters 


### Prerequisites
* Githflow
* Basic HTML and CSS

### Setup
  *Webhint
 NOTE: If you are running on Windows, you need to initialize npm to create package.json file.
```bash
npm init -y
```

1. Run 
```bash
npm install --save-dev hint@7.x
```
2. create a file in the root directory of your project named ```.hintrc``` and copy the following to it
```json
  {
  "connector": {
    "name": "local",
    "options": {
      "pattern": ["**", "!.git/**", "!node_modules/**"]
    }
  },
  "extends": ["development"],
  "formatters": ["stylish"],
  "hints": [
    "button-type",
    "disown-opener",
    "html-checker",
    "meta-charset-utf-8",
    "meta-viewport",
    "no-inline-styles:error"
  ]
}
```
3. Run 
```bash
npx hint .
```
4. Fix validation errors.

### Stylelint
1. Run 
```bash
npm install --save-dev stylelint@13.x stylelint-scss@3.x stylelint-config-standard@21.x stylelint-csstree-validator@1.x
``` 
2. create a file in the root directory of your project named ```.stylelintrc.json``` and copy the following to it

```json
{
  "extends": ["stylelint-config-standard"],
  "plugins": ["stylelint-scss", "stylelint-csstree-validator"],
  "rules": {
    "at-rule-no-unknown": null,
    "scss/at-rule-no-unknown": [
      true,
      {
        "ignoreAtRules": [
          "tailwind",
          "apply",
          "variants",
          "responsive",
          "screen"
        ]
      }
    ]
  },
  "csstree/validator": true,
  "ignoreFiles": ["build/**", "dist/**", "**/reset*.css", "**/bootstrap*.css"]
}
```
3. Run 
```bash
npx stylelint "**/*.{css,scss}"
``` 
  
## Checking 
This is the screenshot that all the thing is okay

