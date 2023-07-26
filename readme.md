# Pinboard
pinboard 更改了源码。
@@ -325,7 +325,7 @@ FILTER."
   "Open the currently-highlighted pin in a web browser."
   (interactive)
   (pinboard-with-current-pin pin
-    (browse-url (alist-get 'href pin))))
+    (eww-browse-url (alist-get 'href pin))))

 (defun pinboard-kill-url ()
   "Add the current pin's URL to the `kill-ring'."
