# pwa-parcel-test
Progressive Web App (https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps) bundled with parcel2 test.

This PWA is made available via:
https://agdturner.github.io/pwa-parcel-test/dist/main/

Dependencies:
1. Node

Installation:
1. Clone the repository
2. cd into the repository
3. Run:
`npm install`

To build run:
`parcel build`

To launch on a local host Web server run:
`npx parcel src/index.html`
 - By default this will run on port 1234. To use a different port for example 2345 run: `npx parcel src/index.html -p 2345`
Once launched, then open http://localhost:1234/ changing the url to match a different port if specified.

Any changes need committing and pushing to the repository for deployment.

To deploy a branch called branch1 to https://agdturner.github.io/pwa-parcel-test/dist/branch1/ edit package.json and change:
```
  "targets": {
    "main": {
      "distDir": "./dist",
      "publicUrl": "/pwa-parcel-test/dist/main/"
    }
  },
```
To:
```
  "targets": {
    "branch1": {
      "distDir": "./dist",
      "publicUrl": "/pwa-parcel-test/dist/branch1/"
    }
  },
```