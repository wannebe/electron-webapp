# 图形化生成

https://github.com/quanglam2807/appifier


# electron-webapp

## Reference

* For Deb: https://github.com/unindented/electron-installer-debian
* For Flatpak: https://github.com/endlessm/electron-installer-flatpak

* electron-packager-interactive: https://github.com/Urucas/electron-packager-interactive
* grunt-electron: https://github.com/sindresorhus/grunt-electron

* electron-packager: https://www.npmjs.com/package/electron-packager
* API: https://github.com/jiahaog/nativefier/blob/master/docs/api.md

* svgtopng: https://github.com/domenic/svg2png


## Installation


1. npm install nativefier -g （安装nativefier）
2. npm install electron --save-dev --save-exact （安装electron）
4. npm install electron-packager -g （安装electron编译包）
5. npm install -g electron-installer-debian （安装electron打deb编译包）
6. sudo apt-get install fakeroot (编译依赖)
7. npm install -g electron-packager-interactive (增强包)
8. npm install svg2png -g (desktop-icon)



## Compile native file

Creating a native desktop app for wechat

> nativefier --name "Wechat" "https://wx.qq.com/"

### Compile deb file

> electron-installer-debian --src /home/deepin/wechat-linux-x64/ --dest /home/deepin/wechat/ --arch amd64

You'll end up with the package at > home/deepin/wechat/wechat-nativefier-4418c7_1.0.0_amd64.deb.
