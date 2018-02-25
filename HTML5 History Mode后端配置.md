#.htaccess（放网站根目录）
```<IfModule mod_rewrite.c>
<IfModule mod_rewrite.c>
  RewriteEngine On
  RewriteBase /
  RewriteRule ^index\.html$ - [L]
  RewriteCond %{REQUEST_FILENAME} !-f
  RewriteCond %{REQUEST_FILENAME} !-d
  RewriteRule . /index.html [L]
</IfModule>
```


#httpd.conf(修改)
```<Directory />
<Directory/>
    #AllowOverride none
    #Require all denied

    Options FollowSymLinks
    AllowOverride None
</Directory>
```

