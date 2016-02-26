A tentative to turn [oojspec](https://github.com/rosenfeld/oojspec/) into a npm package.

# INSTALL

To generate the npm package you have to run the following:

```
npm install
./node_modules/webpack/bin/webpack.js
./node_modules/webpack/bin/webpack.js --config webpack-iframe-runner.config.js
npm pack
```

`npm pack` will generate a file called oojspec-0.0.1.tgz which can be installed with:

```
npm install oojspec-0.0.1.tgz
```

# TODO

* Currently, the vendor files are being compiled altogether. We should grab them from their respective npm packages (for that we have to change oojspec itself, replacing global variables like buster and bane).
