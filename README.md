# Flycheck YAMLLint integration

Flycheck integration for [YAMLLint](https://github.com/adrienverge/yamllint).

# Install
## MELPA
Not available yet.

## Manual
* Download `flycheck-yamllint.el`
* Put it in some directory like `~/.emacs.d/local/`
* Add this code into your Emacs configuration:
```
(add-to-list 'load-path
             (expand-file-name "local" user-emacs-directory))

(require 'flycheck-yamllint)
(eval-after-load 'flycheck
  '(add-hook 'flycheck-mode-hook 'flycheck-yamllint-setup))
```
