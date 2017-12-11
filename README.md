# electron-webapp

## Installation


### sudo npm install nativefier -g
### sudo npm install electron-packager -g
### sudo npm install -g electron-installer-debian
### sudo npm install electron --save-dev --save-exact
### sudo apt-get install fakeroot



## Usage


Creating a native desktop app for ![deepin bbs](bbs.deepin.org)

> nativefier --name "deepinbbs" "https://bbs.deepin.org/"

### Command

> electron-installer-debian --src /home/deepin/wechat-linux-x64/ --dest /home/deepin/wechat/ --arch amd64

You'll end up with the package at > home/deepin/wechat/app_0.0.1_amd64.deb.

### Scripts

> npm install --save-dev electron-installer-debian

Edit the scripts section of your package.json:

``` {
  "name": "app",
  "description": "An awesome app!",
  "version": "0.0.1",
  "scripts": {
    "start": "electron .",
    "build": "electron-packager . app --platform linux --arch x64 --out dist/",
    "deb64": "electron-installer-debian --src dist/app-linux-x64/ --dest dist/installers/ --arch amd64"
  },
  "devDependencies": {
    "electron-installer-debian": "^0.6.0",
    "electron-packager": "^9.0.0",
    "electron": "~1.7.0"
  }
}```

Note: The versions in devDependencies are examples only, please use the latest package versions when possible.

And run the script:

> npm run deb64


## How It Works

* For Deb: https://github.com/unindented/electron-installer-debian
* For Flatpak: https://github.com/endlessm/electron-installer-flatpak


## ![electron-packager ](https://www.npmjs.com/package/electron-packager)
