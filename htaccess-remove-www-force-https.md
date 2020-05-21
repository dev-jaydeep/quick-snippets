# Remove WWW from URL and Force to HTTPS Via htaccess

```
RewriteEngine On

RewriteCond %{HTTP_HOST} ^www.domain.com$ [NC]
RewriteRule ^(.*)$ https://domain.com/$1 [R=301,L]
RewriteCond %{HTTPS} off
RewriteRule (.*) https://%{HTTP_HOST}%{REQUEST_URI} [R,L]
```
