# SHORT FRAMEWORK

## Introduction

The short framework aims to create an alternative tecnology to build web applications using Kotlin, based on the concept of centralizing the full stack of the development into a single repository.
With this concept the it is expected to achieve a better development expirience which leverages the fact that the whole code for the application is in the same code base to implement safe checks between the front-end and back-end of the application, protecting against data missmatches.

## Current status

Currently, to allow for greater flexibility and different development architectures a study is being conducted to split the core package into the following parts:
* HTML DSL (graphical struture of the app)
* JS DSL (functionality of the app's struture)
* APIless (manages calls to the server)
* SPA (converts the app into a single page application)
* SPA-server (deploys as a SPA with APIless)


This division will enable to change the DSLs, architetures(static, SPA, MPA) and resulting representations of the app inside the browser. That implies, multiple configurations to better fit the use cases.


Along with this changes, there is interest to add support for middleware, which will come with some official ones like:
- [ ] SEO populator (populates an HTML with static content on an SPA)
- [ ] Debugger (records server calls, debugs client side code, intented to allow for step-by-step debugging and WASM support)
