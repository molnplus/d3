---
layout: 
title: "Linked Highlighting with React, D3.js and Reflux"

---


安裝過程已經完成。
或者說，根據導航，我認為已經可以了。

來源是
[node management](https://github.com/creationix/nvm)
和[a medium post](https://medium.com/@pbesh/linked-highlighting-with-react-d3-js-and-reflux-16e9c0b2210b#.7bv0s7yrc)

## nodejs
版本管理一直是我不願意面對的，因為不了解，所以有畏懼心理。
目前我採用的方法是nvm。

但是遇到了這樣的問題：

    => You currently have modules installed globally with `npm`. These will no
    => longer be linked to the active version of Node when you install a new node
    => with `nvm`; and they may (depending on how you construct your `$PATH`)
    => override the binaries of modules installed with `nvm`:

    /usr/local/lib
    ├── bower@1.3.3
    ├── coffee-script@1.10.0
    ├── generator-hubot@0.3.1
    ├── grunt@0.4.5
    ├── hubot@2.16.0
    └── yo@1.4.8

    => If you wish to uninstall them at a later point (or re-install them under your
    => `nvm` Nodes), you can remove them from the system Node as follows:

         $ nvm use system
         $ npm uninstall -g a_module

    => Close and reopen your terminal to start using nvm

這或許意味著在使用hubot的時候，需要重新安裝相關的包：

npm install yo
npm install generator-hubot
npm install hubot
npm install coffee-script

需要bower參與的jekyll模板也會受到影響。
暫時先擱置吧。

## Linked Highlighting with React, D3.js and Reflux


npm install yo
npm install react-webpack

yo react-webpack
