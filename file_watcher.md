### Options

| Tables                                                               |                      backend                       |     Used By      |
| -------------------------------------------------------------------- | :------------------------------------------------: | :--------------: |
| [esbuild watch mode](https://github.com/evanw/esbuild)               |                 heuristics pooling                 |     esbuild      |
| [watchpack](https://github.com/webpack/watchpack)                    |                   `graceful-fs`                    |     webpack      |
| [@parcel-bundler/watcher](https://github.com/parcel-bundler/watcher) | FSEvents, Watchman, inotify, ReadDirectoryChangesW | Parcel 2, VSCode |
| [chokidar](https://github.com/paulmillr/chokidar)                    |            Node.js `fs` module, FSEvent            |     webpack      |

### Further Reading:

[esbuild watchmode explain](https://github.com/evanw/esbuild/issues/21#issuecomment-770360728)

[vscode use parcel for watching to avoid consistent cpu usage](https://github.com/microsoft/vscode/commit/e7fffbf1c9169087f1098aedfe54c59c079fa3ac)

[fs.watch triggered twice on fs.writeFile](https://github.com/nodejs/node-v0.x-archive/issues/2054#issuecomment-8686322)

### Further Thinking:

- How to deal with large codebase changes when developer checkout a bunch of new code ?
