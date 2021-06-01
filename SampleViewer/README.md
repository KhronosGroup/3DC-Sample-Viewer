glTF Certification Viewer Web App
=================================

Requirements
------------

- Node.js
- npm

Setup
-----

For local usage and debugging, please follow these instructions:

0. Make sure [Git LFS](https://git-lfs.github.com) is installed.

1. Checkout the [`main`](../../tree/main) branch

2. Build the viewer
	- `cd SampleViewer`
	- run `npm install`
	- start a demo in the browser with `npm run dev`, and open http://localhost:8000.

When making changes, the project is automatically rebuilt and the `SampleViewer/dist/` directory is populated with the viewer. This directory contains all files necessary for deployment to a webserver.

Debugging
---------

* Requirements
  * [Visual Studio Code](https://code.visualstudio.com/) or [vscodium](https://github.com/VSCodium/vscodium)
  * [Chrome](https://www.google.com/chrome/) or [Firefox](https://www.mozilla.org/en-US/firefox/new/)
* Install the [Debugger for Chrome](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome) or [Debugger for Firefox](https://marketplace.visualstudio.com/items?itemName=hbenl.vscode-firefox-debug) extension for Visual Studio Code
* Open the project directory in Visual Studio Code and select `Debug->Add Configuration->Chrome` or `Debug->Add Configuration->Firefox` so the `.vscode/launch.json` file is created.
* Append `/SampleViewer/dist` to `${workspaceFolder}` in the `launch.json` file
* `Debug->Start Debugging` should now launch a Chrome or Firefox window with the sample viewer and VS Code breakpoints should be hit.