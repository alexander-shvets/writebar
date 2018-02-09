<p align="center"><a href="//writebar.js.org" title="writebar.js.org"><img src="assets/logo.svg"/></a></p>
<h1 align="center">WriteBar</h1>
<p align="center">
  Experimental distraction-free text editor,<br/>
  that displays focus text line right over the keyboard (on the Macbook Pro TouchBar).
</p>
<h2 align="center"><a href="dist/WriteBar.dmg">
  Download (dmg)
</a></h2>
<p align="center"><img width="600" src="assets/screenshot.jpg" alt="screenshot"/></p>

### Discuss

- [Feature Requests and Issues](//github.com/alexander-shvets/writebar/issues)     
- [Intro post on UX Club](//facebook.com/groups/uxclubs/permalink/973396292808999/)

## Development

Download source code:    
```shell
git clone git@github.com:alexander-shvets/writebar.git
cd writebar
```

Install macOS package manager ([Homebrew][]):
```shell
brew || /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Install Node package manager ([yarn][]):
```shell
yarn || brew install yarn
```

Install application dependencies:
```shell
yarn
```

Install (global or local) dev-dependencies*:    
```shell
yarn global add electron
yarn global add electron-packager
yarn global add electron-installer-dmg
```
_* doesn't listed in [`package.json`][] becouse I doesn't use js builder yet (which will exclude unused dependencies from application installation package)_

Run app in dev mode:    
```shell
yarn start
```

Build app and Installer:    
```shell
yarn build
```
Release files generated in [`dist`][] directory.

[`package.json`]: //github.com/alexander-shvets/writebar/blob/master/package.json
[`dist`]: //github.com/alexander-shvets/writebar/tree/master/dist
[Homebrew]: //brew.sh
[yarn]: //yarnpkg.com

