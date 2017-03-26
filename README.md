# Flycheck YAMLLint integration

Flycheck integration for [YAMLLint](https://github.com/adrienverge/yamllint).

# Install
## use-package (recommended)
Add this code into your Emacs configuration:
```
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
```
(require 'flycheck-yamllint)
(eval-after-load 'flycheck
  '(add-hook 'flycheck-mode-hook 'flycheck-yamllint-setup))
```

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
