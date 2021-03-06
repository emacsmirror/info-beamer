# Emacs minor mode for info-beamer

[![Melpa](https://melpa.org/packages/info-beamer-badge.svg)](https://melpa.org/#/info-beamer)
[![Melpa Stable](https://stable.melpa.org/packages/info-beamer-badge.svg)](https://stable.melpa.org/#/info-beamer)
[![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html)

This package provides utilities for working with [info-beamer](https://info-beamer.com/opensource).

## Features

* Run your info-beamer node
* Lookup documentation
* Send data to your info-beamer node via
  - TCP
  - UDP
  - OSC

## Configuration

See the `info-beamer` customization group for settings:
`M-x customize-group RET info-beamer`

To turn on `info-beamer-mode` in all Lua buffers:

``` emacs-lisp
(use-package info-beamer
  :hook (lua-mode . info-beamer-mode))
```

## Usage

| Key                | Command             |
|--------------------|---------------------|
| <kbd>C-c ' !</kbd> | info-beamer-run     |
| <kbd>C-c ' r</kbd> | info-beamer-run     |
| <kbd>C-c ' ?</kbd> | info-beamer-doc     |
| <kbd>C-c ' h</kbd> | info-beamer-doc     |
| <kbd>C-c ' c</kbd> | info-beamer-connect |
| <kbd>C-c ' t</kbd> | info-beamer-input   |
| <kbd>C-c ' i</kbd> | info-beamer-input   |
| <kbd>C-c ' u</kbd> | info-beamer-data    |
| <kbd>C-c ' d</kbd> | info-beamer-data    |
| <kbd>C-c ' o</kbd> | info-beamer-osc     |
