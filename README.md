![GPLv3](https://img.shields.io/badge/license-GPLv3-brightgreen.svg)
[![MELPA](https://melpa.org/packages/0xc-badge.svg)](https://melpa.org/#/0xc)
[![Build Status](https://travis-ci.org/AdamNiederer/0xc.svg?branch=master)](https://travis-ci.org/AdamNiederer/0xc)
![Coverage](https://img.shields.io/badge/coverage-83%25-green.svg)

# 0xc
(Pronounced "hex convert")

Base conversion made easy in emacs

## Features
- Base conversion!
- Intelligent base inference
- Replace-at-point methods
- Simple representation of bases up to 36

## Installation & Setup
0xc is avilable on [Melpa](https://melpa.org/#/0xc). After installing with `M-x package-install <RET> 0xc <RET>`,
all functions should be available.

## Functions
- `0xc-convert` - Simple string-to-string base conversion. Accepts prefix options and allows interactive use.
- `0xc-convert-point` - Replace the number at point with a converted representation.

## Base Hinting

A number literal's base can be roughly determined via heuristics, but you can use the following hints to ensure 0xc gets it right:

- `0x` is a hexadecimal literal
- `0b` is a binary literal
- `0t` is a ternary literal
- `0d` is a decimal literal
- `0o` is an octal literal

Alternatively, you can prefix a base-n number with `n:`. 0xc will automatically remove any of these base hints when converting

## Future
More tests are next. If you feel like beating me to it, open a pull request.

## License
GPLv3+
