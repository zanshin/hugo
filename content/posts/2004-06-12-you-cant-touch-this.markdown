--- 
layout: post
title: You Can't Touch This
date: 2004-06-12T03:02:00
comments: true
tags:
- life
link: false
---
Thanks to <a href="http://www.padawan.info/" title="padawan.info">padawan.info</a>'s <a href="http://www.padawan.info/weblog/preventing_image_hotlinking.html" title="preventing image hotlinking">preventing image hotlinking</a> article I now have protected to some degree my site's images.

The process is relatively simple, create a new .htaccess file for your images subfolder (you do have an images subfolder, right?) and paste the following code in it.
{{< highlight bash  >}}
RewriteEngine On
RewriteCond %{HTTP_REFERER} !^$
RewriteCond %{HTTP_REFERER} !^http://(www.)?zanshin.net(/)?.*$ [NC]
RewriteRule .*.(gif|jpg|jpeg|png)$ - [F,NC]{{< / highlight >}}
Cool.
