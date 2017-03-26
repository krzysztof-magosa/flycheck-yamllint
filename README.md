# Flycheck YAMLLint integration
[![MELPA](https://melpa.org/packages/flycheck-yamllint-badge.svg)](https://melpa.org/#/flycheck-yamllint)
[![MELPA Stable](https://stable.melpa.org/packages/flycheck-yamllint-badge.svg)](https://stable.melpa.org/#/flycheck-yamllint)

Flycheck integration for [YAMLLint](https://github.com/adrienverge/yamllint).

# Install
## use-package (recommended)
Add this code into your Emacs configuration:
```elisp
(use-package flycheck-yamllint
  :ensure t
  :defer t
  :init
  (progn
    (eval-after-load 'flycheck
      '(add-hook 'flycheck-mode-hook 'flycheck-yamllint-setup))))
```

## MELPA
* Press `M-x`, type package-install
* Specify `flycheck-yamllint`
* Add this code into your Emacs configuration:
```elisp
(require 'flycheck-yamllint)
(eval-after-load 'flycheck
  '(add-hook 'flycheck-mode-hook 'flycheck-yamllint-setup))
```

## Manual
* Download `flycheck-yamllint.el`
* Put it in some directory like `~/.emacs.d/local/`
* Add this code into your Emacs configuration:
```elisp
(add-to-list 'load-path
             (expand-file-name "local" user-emacs-directory))

(require 'flycheck-yamllint)
(eval-after-load 'flycheck
  '(add-hook 'flycheck-mode-hook 'flycheck-yamllint-setup))
```
