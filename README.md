# electron-webapp

## Installation


### npm install nativefier -g
### npm install electron-packager -g
### npm install -g electron-installer-debian
### npm install electron --save-dev --save-exact
### sudo apt-get install fakeroot

### npm install -g electron-packager-interactive 增强



## Usage


Creating a native desktop app for ![deepin bbs](bbs.deepin.org)

> nativefier --name "deepinbbs" "https://bbs.deepin.org/"

### Command

> electron-installer-debian --src /home/deepin/wechat-linux-x64/ --dest /home/deepin/wechat/ --arch amd64

You'll end up with the package at > home/deepin/wechat/app_0.0.1_amd64.deb.


## How It Works

* For Deb: https://github.com/unindented/electron-installer-debian
* For Flatpak: https://github.com/endlessm/electron-installer-flatpak
* electron-packager-interactive: https://github.com/Urucas/electron-packager-interactive
* grunt-electron: https://github.com/sindresorhus/grunt-electron

* electron-packager: https://www.npmjs.com/package/electron-packager

* API: https://github.com/jiahaog/nativefier/blob/master/docs/api.md
