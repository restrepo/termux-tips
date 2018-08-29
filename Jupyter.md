## Installing jupyter with numpy matplotlib and pands
see [here](https://www.leouieda.com/blog/scipy-on-android.html)
```bash
dpkg install clang python python-dev fftw libzmq libzmq-dev freetype freetype-dev libpng libpng-dev pkg-config
LDFLAGS=" -lm -lcompiler_rt" pip install numpy matplotlib pandas jupyter
```
Next
```bash
jupyter-notebook
```
and copy and paste the localhost URL into Google Chrome

## Installing scipy
See [Installing Scipy The Easy Way](https://wiki.termux.com/wiki/Installing_Scipy_The_Easy_Way)

1. Prepare repo
```bash
pkg install wget
$PREFIX/bin/wget https://its-pointless.github.io/setup-pointless-repo.sh
bash setup-pointless-repo.sh
```
2. Install Scipy: (not with `pip`)
```bash
pkg install scipy
```
## Install codeboard
[CodeBoard Keyboard for Coding](https://play.google.com/store/apps/details?id=com.gazlaws.codeboard&hl=en)
May be also the [Hakcker's keyboard](https://play.google.com/store/apps/details?id=org.pocketworkstation.pckeyboard) in which the combination `<Shift>+<Enter>` works

## Launch jupyter
From the termux, launch `jupyter-notebook` and copy the URL
<img source="./img/jupyter.png" width="200"/>

## Manage your termux "operating system" from jupyter
Paste the URL into Google Chrome. 
*  From there you can  have access to the termux filesystem with delete and upload/download of files, editor, PDF viewer, ,  etc.
<img source="./img/chrome1.png" width="200"/>

* Code cells include an execution button. Working with the toolbar is also convenient.
<img source="./img/chrome2.png" width="200"/>

