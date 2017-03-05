# Env3D Javascript Transpiler

## Usage

Make sure you edit the beginning of build.gradle file with the correct directories,
then run:

```
gradle dist
```

## Background

The goal of this project is to take .java files in the env3d environment and
tranpile them into .js files to be used in the webgl environment.

In conjunction with the [env3d-js](https://github.com/env3d/env3d-js) project, 
program written for the desktop env3d version can now run in the browser 
without plugins, etc.

Furthermore, Android and iOS apps can be created by using webview-based
native app generators such as [Apache Cordova](https://cordova.apache.org/).

## The shim
The env3d-shim-0.0.1-SNAPSHOT.jar file in the libs/ directory allows 
the traspilation to happen, but the actual env3d.js library is not
transpiled, but rather re-written using [threejs](https://threejs.org/).
