# electron-webapp

## Installation


### npm install nativefier -g
### npm install electron-packager -g
### npm install -g electron-installer-debian



## Usage


Creating a native desktop app for ![deepin bbs](bbs.deepin.org)

> nativefier --name "deepinbbs" "https://bbs.deepin.org/"

### You now run electron-packager to build the app for Debian:

> electron-packager . app --platform linux --arch x64 --out dist/

### If you want to run electron-installer-debian straight from the command-line, install the package globally:

> npm install -g electron-installer-debian

### And point it to your built app:

> electron-installer-debian --src dist/app-linux-x64/ --dest dist/installers/ --arch amd64

You'll end up with the package at > dist/installers/app_0.0.1_amd64.deb.



## How It Works

* For Deb: https://github.com/unindented/electron-installer-debian
* For Flatpak: https://github.com/endlessm/electron-installer-flatpak


## ![electron-packager ](https://www.npmjs.com/package/electron-packager)
