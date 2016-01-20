# discover-chromecasts [![NPM version](http://img.shields.io/npm/v/discover-chromecasts.svg?style=flat-square)](https://www.npmjs.org/package/discover-chromecasts)

Discover/detect all Chromecast devices on a network.

## Installation

Install the package with NPM:

```bash
$ npm install discover-chromecasts
```

## Usage

Example:

```javascript
import discoverChromecasts from "discover-chromecasts";

discoverChromecasts({ timeout: 5000 })
.then(chromecasts => {
  chromecasts.forEach(chromecast => {
    console.log(chromecast);
  });
}).catch(err => {
  console.error(err.message);
});
```

## Disclaimer

The tool is not officially affiliated with Google in any way. Use at own risk.

Code originally forked from [chromecast-scanner](https://github.com/xat/chromecast-scanner).
