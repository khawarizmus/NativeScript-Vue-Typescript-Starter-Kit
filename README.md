# NativeScript-Vue Typescript Starter Kit

<p align="center">
  <img alt="Logo" src="./app/assets/images/NativeScript-Vue.png" height="157" />
</p>

> A NativeScript-Vue + Typescript starter kit for getting up and running quickly

[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

<div align="center">
    <img alt="Logo" src="https://i.imgur.com/GerflS3.png" />
</div>

# What do you get

This starter kit aims to make your development environment as efficient as possible, by having typescript integrated into our project we benefit from the language powerful features like, type checking, great tooling with IntelliSense support and a pure OOP paradigm.

This kit is [commitizen](https://github.com/commitizen/cz-cli) friendly and uses [commitlint](https://github.com/marionebl/commitlint), it comes with automated [sementic-relese](https://github.com/semantic-release/semantic-release) out of the box with Github [changlog](https://github.com/semantic-release/github) automated generation.

This kit uses [ts-loader](https://github.com/TypeStrong/ts-loader) which is a typescript loader for webpack , [fork-ts-checker-webpack-plugin](https://github.com/Realytics/fork-ts-checker-webpack-plugin) for a better performance and offers you with [vue-property-decorator](https://github.com/kaorun343/vue-property-decorator) to get the most out of typescript in your vue files.

# Usage

We assume that you have all the [prerequisites](https://nativescript-vue.org/en/docs/getting-started/installation/#prerequisites) installed


Then You first need to clone the repo to your local machine

```bash
git init
git clone https://github.com/gimyboya/NativeScript-Vue-Typescript-Starter-Kit.git
```
Once done you need to point the remote origin to your own git repository

```bash
git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```
Then install the your packages

```bash
# Install dependencies
npm install
```

### Scripts

The following scripts are available for you to run and build your application
**Note:** <platform> can be either `android` or `ios`

``` bash

# to commit your changes using commitizen (important)
npm run commit

# run you app
npm run run:<platform>

# clean run your app
npm run clean-run:<platform>

# run with hot module reloading
npm run watch:<platform>

# build your app
npm run build:<platform>
    
```
# Contribution

**NOTE:** This repo is commitizen friendly that follows [AngularJS's commit message convention](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) also known as [conventional-changelog](https://github.com/ajoslin/conventional-changelog).

Contributions are welcomed.