# NodeGateway
English | [简体中文](./README-zh.md)

## Introduction

NodeGateway is blockchain node access service platform similar to infrua on Ethereum which is a public blockchain（will support FIL、ETH etc）node access service for developers. Developers who want to develop DAPP in FVM or other application can use NodeGateway API to interact with the chain without deploying their own blockchain nodes.We will technically guarantee its strong and stable performance.Assuming that the developer has already use FIL node which they deployed self before, they can access the NodeGateway only by modifying the URL without changing the interface.

## Website

https://node-gateway.storeros.com/console/#/

username:test

password:test

**Note:** Under development, the function is not perfect

## Build Setup

```bash
# clone the project
git clone https://github.com/StorerOS/NodeGateway.git

# enter the project directory
cd NodeGateway

# install dependency
yarn install

# develop
yarn dev
```

This will automatically open http://localhost:9528

## Build

```bash
# build for test environment
yarn build:stage

# build for production environment
yarn build:prod
```

## Advanced

```bash
# preview the release environment effect
yarn preview

# preview the release environment effect + static resource analysis
yarn preview -- --report

# code format check
yarn lint

# code format check and auto fix
yarn lint -- --fix
```

## Browsers support

Modern browsers and Internet Explorer 10+.

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](http://godban.github.io/browsers-support-badges/)</br>Safari |
| --------- | --------- | --------- | --------- |
| IE10, IE11, Edge| last 2 versions| last 2 versions| last 2 versions
