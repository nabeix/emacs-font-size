# emacs-font-size
Change frame font size dynamically

## Overview

`font-size.el` provides the features to change frame font size.

The difference between the built-in `text-scale-adjust` and `font-size.el` is a scope of applying.

The `text-scale-adjust` changes the font size of the text of a particular buffer, and doesn't target the mode line and minibuffer.

But, `font-size.el` targets all text of a frame.

![font-size-change](images/font-size-change.gif)

## Installation

Get `font-size.el` and install it to load-path directory.

## Usage

```
(require `font-size)
(font-size-init 16)
```

`font-size.el` provides:

* font-size-change
  * changes the font size interactive
* font-size-decrease
  * decreseas the font size
* font-size-increase
  * increases the font size
* font-size-default
  * change the font size to default

The following is an example key-binding definition like Mac OS Applications.

```
(define-key global-map (kbd "M-+") 'font-size-increase)
(define-key global-map (kbd "M--") 'font-size-decrease)
(define-key global-map (kbd "M-0") 'font-size-default)
```

## Contribution

1. Fork it ( http://github.com/nabeix/emacs-font-size )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create new Pull Request

## License

GPL v3
