#Signal nw.js

[nw.js](http://nwjs.io/) provides for easily running Chrome applications
in it's native app containers (which ship Node and all application files
as a standard platform native application.

##Building a Signal Desktop packaged application

First you need to install the NW builder:

```
npm install -g nw-builder
```

There's a shell script called `package.sh` which will prepare this repo to
produce a packaged app. So just do:

```
./package.sh
```

and then you should be able to execute

```
nwbuild -p Linux64 .
```

to build a package!

##Manually running signal in nw.js

If you want to do this yourself you can do the following (after installing
[nw.js](http://nwjs.io/):

```
git clone git@github.com:WhisperSystems/Signal-Desktop.git
cd Signal-Desktop
npm install
grunt
nw ./dist
```

and that's it!
