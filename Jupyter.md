# Jupyter in android
After [install Termux](./termux.md):

## Installing Jupyter with NumPy, Matplotlib and Pandas

see [here](https://www.leouieda.com/blog/scipy-on-android.html)
```bash
dpkg install clang python python-dev fftw libzmq libzmq-dev freetype freetype-dev libpng libpng-dev pkg-config

LDFLAGS=" -lm -lcompiler_rt" pip install numpy matplotlib pandas jupyter
```

## Installing SciPy
See [Installing Scipy The Easy Way](https://wiki.termux.com/wiki/Installing_Scipy_The_Easy_Way)

1. Prepare repo
```bash
pkg install wget
wget https://its-pointless.github.io/setup-pointless-repo.sh
bash setup-pointless-repo.sh
```
2. Install Scipy: (not with `pip`)
```bash
pkg install scipy
```
## Install extended keyboard
Use [Hacker's keyboard](https://github.com/klausw/hackerskeyboard). Go to the settings and choose the full 5-row keyboard in portrait mode‘:

<img src="./img/hackerskbd.png" width="250"/>

which works like a desktop keyboard. In particular,  the combination `<Shift>+<Enter>`.

The others keyboards with bigger keys, can be easily actived by using the volume down key.



You May also consider the [CodeBoard Keyboard for Coding](https://play.google.com/store/apps/details?id=com.gazlaws.codeboard&hl=en).

## Launch jupyter
From the termux execute the command
```bash
jupyter-notebook
```
and copy the URL

<img src="./img/jupyter.png" width="250"/>

* Touching the upper left edge of the screen you have acces to the termux options to open new sessions and toogle to other sessions. 
## Manage your termux "operating system" from jupyter
Paste the URL into Google Chrome. 
*  From there you can  have access to the termux filesystem with delete and upload/download of files, editor, PDF viewer, ,  etc.
<img src="./img/chrome1.png" width="250"/>

* Code cells include an execution button. Working with the toolbar is also convenient.
<img src="./img/chrome2.png" width="250"/>

