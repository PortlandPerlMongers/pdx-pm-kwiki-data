[[TomHeady]]

    ;; If running under screen, disable C-z.
    (if (and (getenv "STY") (not window-system))
         (global-unset-key "\C-z"))

    (global-set-key "\M-g" 'goto-line) ;; alt-g <line> enter goes to line

    [http://www.northbound-train.com/emacs-hosted/backup-dir.el download backup-dir.el]

    ;; backup files to a backup directory
    (require 'backup-dir)

    (make-variable-buffer-local 'backup-inhibited)  ;; localize it for safety.
    (setq bkup-backup-directory-info
          '((t "~/.emacs.d/backup" ok-create full-path prepend-name)))
    (setq delete-old-versions t
          kept-old-versions 1
          kept-new-versions 3
          version-control t)
