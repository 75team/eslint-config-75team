# eslint-config-75team
> The recommended eslint config of 75team

[![npm](https://img.shields.io/npm/v/eslint-config-75team.svg?style=flat-square)](https://www.npmjs.com/package/eslint-config-75team)[![dependency status](https://david-dm.org/75team/esint-config-75team.svg)](https://david-dm.org/75team/esint-config-75team) [![License](https://img.shields.io/npm/l/eslint-config-75team.svg)](LICENSE)



Extends `eslint-config-airbnb-base`.
Use it as is or as a foundation for your own config.

To see the rules that this config uses, please read the detail of our [config rules](https://github.com/75team/eslint-config-75team/blob/master/index.js).

## Installation

``` bash
npm install eslint eslint-config-75team --save-dev
```

## Usage

Once you installed `eslint-config-75team` locally within you project, just set you eslint config to :

``` json
{
    "extends":  "eslint-config-75team"
}
```
Since we have extended `'stylelint-config-standard'`, you don't need to install the standard extends again.

## How the customize your own rules

Simply add a "rules" key to your config, then add your overrides and additions there.

For example, if you want the max param number in a function to be 6, just add `'max-params': ['error', 6],` to rules

``` json
{
    "extends":  "eslint-config-75team",
    "rules": {
        "max-params": ["error", 5]
    }
}
```

If you need furthor information about customizing rules, you can read [configuration guide](https://eslint.org/docs/user-guide/configuring) and [rules of eslint](https://eslint.org/docs/rules/)

## Use in IDE

If you want to use eslint in your project, we suggest you use the corresponding plugin in your IDE to get better coding experience.

### VSCode
If you use VSCode, you need to install the following plugins:

1. **[eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)**: Integrates ESLint into VS Code.

### Sublime

If you use Sublime, you need to install **SublimeLinter** and **SublimeLinter-contrib-eslint**

In order for eslint to be executed by SublimeLinter,you must ensure that nodejs is available to SublimeLinter.Before going any further, please read and follow the steps in “[Finding a linter executable](http://sublimelinter.readthedocs.io/en/latest/troubleshooting.html#finding-a-linter-executable)” through “Validating your PATH” in the documentation.