# WAM Website — WatchYourNet LTD

Static responsive website for WAM / WatchYourNet LTD.

## Files
- `index.html`
- `styles.css`
- `script.js`

## Deployment
Upload these files to the document root for `watchyour.net` or serve them with nginx/Apache.

Example nginx root:

```nginx
server {
    listen 443 ssl http2;
    server_name watchyour.net www.watchyour.net;
    root /var/www/watchyour.net;
    index index.html;

    location / {
        try_files $uri $uri/ /index.html;
    }
}
```

Update TLS settings to match the server's certificate configuration.
