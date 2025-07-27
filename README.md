<!-- markdownlint-configure-file {
  "MD013": {
    "code_blocks": false,
    "tables": false,
    "line_length":200
  },
  "MD033": false,
  "MD041": false
} -->

[license]: /LICENSE
[license-badge]: https://img.shields.io/github/license/jerrykuku/luci-theme-argon?style=flat-square&a=1
[prs]: https://github.com/jerrykuku/luci-theme-argon/pulls
[prs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[issues]: https://github.com/jerrykuku/luci-theme-argon/issues/new
[issues-badge]: https://img.shields.io/badge/Issues-welcome-brightgreen.svg?style=flat-square
[release]: https://github.com/jerrykuku/luci-theme-argon/releases
[release-badge]: https://img.shields.io/github/v/release/jerrykuku/luci-theme-argon?style=flat-square
[download]: https://github.com/jerrykuku/luci-theme-argon/releases
[download-badge]: https://img.shields.io/github/downloads/jerrykuku/luci-theme-argon/total?style=flat-square
[contact]: https://t.me/jerryk6
[contact-badge]: https://img.shields.io/badge/Contact-telegram-blue?style=flat-square
[en-us-link]: /README.md
[zh-cn-link]: /README_ZH.md
[en-us-release-log]: /RELEASE.md
[zh-cn-release-log]: /RELEASE_ZH.md
[config-link]: https://github.com/jerrykuku/luci-app-argon-config/releases
[lede]: https://github.com/coolsnowwolf/lede
[official]: https://github.com/openwrt/openwrt
[immortalwrt]: https://github.com/immortalwrt/immortalwrt

<div align="center">
<img src="https://firebasestorage.googleapis.com/v0/b/discord-cdn-sucks.appspot.com/o/image%2Fupper.jpg?alt=media" style="border-radius: 16px; margin-bottom: 8px;">

Argon is **a clean and tidy OpenWrt LuCI theme** that allows<br/>
users to customize their login interface with images or videos.  
It also supports automatic and manual switching between light and dark modes.

All rights & credits to [jerrykuku](https://github.com/jerrykuku), the creator of this Theme.

[![license][license-badge]][license]
[![prs][prs-badge]][prs]
[![issues][issues-badge]][issues]
[![release][release-badge]][release]
[![download][download-badge]][download]
[![contact][contact-badge]][contact]

[Key Features](#key-features) •
[Branch](#branch-introduction) •
[Version History](#version-history) •
[Getting started](#getting-started) •
[Screenshots](#screenshots) •
[Contributors](#contributors) •
[Credits](#credits)
</div>

## Key Features

- Clean Layout.
- Adapted to mobile display.
- Customizable theme colors.
- Support for using Bing images as login background.
- Support for custom uploading of images or videos as login background.
- Automatically switch between light and dark modes with the system, and can also be set to a fixed mode.
- Settings plugin with extensions [luci-app-argon-config][config-link]
- Background inside OpenWrt LuCI panel (New)
- Modified sidebar orientation (Updated)

## Getting started

### Build for OpenWrt official SnapShots and ImmortalWrt

```bash
cd openwrt/package
git clone https://github.com/1121gbps/luci-theme-argon.git
make menuconfig #choose LUCI->Theme->Luci-theme-argon
make -j1 V=s
```

### Install for OpenWrt official SnapShots and ImmortalWrt

```bash
opkg update
opkg install luci-compat
opkg install luci-lib-ipkg
wget --no-check-certificate https://github.com/1121gbps/luci-theme-argon/releases/download/v2.5.2/luci-theme-argon_2.5.2-r20250726_all.ipk
opkg install luci-theme-argon*.ipk
```

### Install luci-app-argon-config

```bash
wget --no-check-certificate -O luci-app-argon-config_1.2_all.ipk https://github.com/1121gbps/luci-theme-argon/releases/download/v2.5.2/luci-app-argon-config_1.2_all.ipk
opkg install luci-app-argon-config*.ipk
```

## Notice

- Chrome browser is highly recommended. There are some new css3 features used in this theme, currently only Chrome has the best compatibility.
- Microsoft has officially retired Internet Explorer, RIP IE🙏<del>Currently, the mainline version of the IE series has bugs that need to be addressed.</del>
- FireFox does not enable the backdrop-filter by default, [see here](https://developer.mozilla.org/zh-CN/docs/Web/CSS/backdrop-filter) for the opening method.
- For changing background inside LuCI Dashboard, **navigate to System > Argon Config > Background Image Path (Inside dashboard).** Add or change background as you needs. Make sure to put your custom background inside **/www/luci-static/argon/background/**
- Background Image Path is Case-Sensitive, make sure you're putting correct file name.

## Screenshots
<img src="https://firebasestorage.googleapis.com/v0/b/discord-cdn-sucks.appspot.com/o/image%2Fscreenshot-pc.jpg?alt=media" style="border-radius: 16px; margin-bottom: 8px;">

## Contributors

<a href="https://github.com/jerrykuku/luci-theme-argon/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=jerrykuku/luci-theme-argon&v=2" />
</a>

Made with [contrib.rocks](https://contrib.rocks).

## Credits

[luci-theme-material](https://github.com/LuttyYang/luci-theme-material/) | 
[jerrykuku](https://github.com/jerrykuku)
