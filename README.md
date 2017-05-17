# [GitHub Desktop](https://desktop.github.com)

[![Travis Build Status](https://travis-ci.com/desktop/desktop.svg?token=bruh3Kp8xZqr5CQ5et3q&branch=master)](https://travis-ci.com/desktop/desktop) [![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/kstdl28ba3f7drbr/branch/master?svg=true)](https://ci.appveyor.com/project/github-windows/desktop/branch/master)

GitHub Desktop is an open source [Electron](https://electron.atom.io)-based
GitHub app. It is written in [TypeScript](http://www.typescriptlang.org) and
uses [React](https://facebook.github.io/react/).

### Linux port 🐧

This is a work in progress port to Linux. My current setup:
```
💩👻~ $ node --version
v7.10.0
💩👻~ $ npm --version
4.2.0
💩👻~ $ python --version
Python 2.7.13
💩👻~ $ cat /etc/issue
Debian GNU/Linux 9
```

You need to install `libsecret-1-0` and `libsecret-1-dev`. On Debian systems:

```
$ sudo apt-get install libsecret-1-0 libsecret-1-dev
```

I haven't managed to start the app with `npm start` yet. But `npm install` and `npm run build:dev` work fine, and you can start the app with `node script/start`. There's also a small hack on script/run.js which adds the '-dev' string to the binary's path. I assume this is necessary due to my lack of knowledge of the whole Node/Electron setup, and may probably be fixed.

![GitHub Desktop on Linux](https://cloud.githubusercontent.com/assets/689327/26164874/6c2b8920-3b04-11e7-8d4e-f1db027cb4a2.jpg)

![GitHub Desktop screenshot - Windows](https://cloud.githubusercontent.com/assets/359239/26094502/a1f56d02-3a5d-11e7-8799-23c7ba5e5106.png)

## Where can I get it?

Download the installer for your OS:

 - [macOS](https://central.github.com/deployments/desktop/desktop/latest/darwin)
 - [Windows](https://central.github.com/deployments/desktop/desktop/latest/win32)
 - [Windows machine-wide install](https://central.github.com/deployments/desktop/desktop/latest/win32?format=msi)

You can install this alongside your existing GitHub Desktop for Mac or GitHub
Desktop for Windows application.

**NOTE**: there is no current migration path to import your existing
repositories into the new application - you can drag-and-drop your repositories
from disk onto the application to get started.


## I have a problem with GitHub Desktop

First, please search the [open issues](https://github.com/desktop/desktop/issues?q=is%3Aopen)
and [closed issues](https://github.com/desktop/desktop/issues?q=is%3Aclosed)
to see if your issue hasn't already been reported (it may also be fixed).

If you can't find an issue that matches what you're seeing, open a [new issue](https://github.com/desktop/desktop/issues/new)
and fill out the template to provide us with enough information to investigate
further.

## How can I contribute to GitHub Desktop?

The [CONTRIBUTING.md](./CONTRIBUTING.md) document will help you get setup and
familiar with the source. The [documentation](docs/) folder also contains more
resources relevant to the project.

If you're looking for something to work on, check out the [up-for-grabs](https://github.com/desktop/desktop/issues?q=is%3Aopen+is%3Aissue+label%3Aup-for-grabs) label.

## More Resources

See [desktop.github.com](https://desktop.github.com) for more product-oriented
information about GitHub Desktop.

## License

**[MIT](LICENSE)**

The MIT license grant is not for GitHub's trademarks, which include the logo
designs. GitHub reserves all trademark and copyright rights in and to all
GitHub trademarks. GitHub's logos include, for instance, the stylized
Invertocat designs that include "logo" in the file title in the following
folder: [logos](app/static/logos).

GitHub® and its stylized versions and the Invertocat mark are GitHub's
Trademarks or registered Trademarks. When using GitHub's logos, be sure to
follow the GitHub [logo guidelines](https://github.com/logos).
