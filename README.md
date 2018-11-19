# Electron Comrade

Electron Comrade is a CLI tool that allows you to run Electron apps with
different versions of Electron. This is useful during development and testing,
enabling you to quickly test a built app with different versions of Electron or
even custom builds.

## Usage

```sh
electron-comrade --electron path/to/electron --app path/to/app
```

 * `-e, --electron`: Version of Electron or path to an Electron build or distribution
 * `-a, --app`: Path to an app or a static build of an app (see below)

### Examples

Windows: Running an installed app with a different version of Electron

```powershell
electron-comrade --electron 3.0.9 --app ~\AppData\Local\slack\app-3.3.4\
```

## Static App Build

A static app build is an Electron app, minus all of Electron. This is usually
everything that'd you find in your app's resources folder. Instead of passing
a fully installed app, you can also pass said static build - the folder
containing `electron.asar` and the rest of your app.

## License
MIT, please see LICENSE for details.
