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
