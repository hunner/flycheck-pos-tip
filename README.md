# flycheck-pos-tip

This is extension for [Flycheck](https://github.com/flycheck/flycheck).
This extension to display errors under point using [pos-tip](https://github.com/syohex/pos-tip).

![Emacs Screenshot with flycheck-pos-tip](https://github.com/flycheck/flycheck-pos-tip/raw/master/screenshot.png)

## Installation

As usual, from [MELPA](https://melpa.org).

In your [Cask](http://cask.github.io) file:

```cl
(source gnu)
(source melpa)

(depends-on "flycheck-pos-tip")
```

In your `init.el`:

```cl
(eval-after-load 'flycheck
  '(custom-set-variables
   '(flycheck-display-errors-function #'flycheck-pos-tip-error-messages)))
```

## Usage

### Configure

```
(custom-set-variables
 '(flycheck-pos-tip-timeout 10))
```

## License

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program.  If not, see http://www.gnu.org/licenses/.

See
[COPYING](https://github.com/flycheck/flycheck-pos-tip/blob/master/COPYING)
for details.
