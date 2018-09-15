## LaTeX in Termux
Minimal install
```bash
dpkg install texlive
```
To have a minimal set of fonts
```bash
fmtutil --all
```
To install missing packages use
```bash
tlmgr install PACKAGE
```
Possibles `PACKAGE`s include:
```
xcolor siunitx l3kernel l3packages cancel todonotes xkeyval pgf comment
```

## Using emacs

Install AucTeX with `<Esc>+x list-packages`.

To install cdLaTeX-mode, install first `el-get` by including in `~/.emacs`
```lisp
(add-to-list 'load-path "~/.emacs.d/el-get/el-get")

(unless (require 'el-get nil 'noerror)
  (with-current-buffer
      (url-retrieve-synchronously
       "https://raw.githubusercontent.com/dimitri/el-get/master/el-get-install.el")
    (goto-char (point-max))
    (eval-print-last-sexp)))

(add-to-list 'el-get-recipe-path "~/.emacs.d/el-get-user/recipes")
(el-get 'sync)
```

To keep the usual AucTex math prefix, it is neccessary to deactivate the cdLaTeX one by adding to the `~/.emacs`
```lisp
(setq cdlatex-math-symbol-prefix [f7])
```