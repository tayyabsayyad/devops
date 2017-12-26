
# Git proxy server configuration

## To set the Proxy Server

$ git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080

- Change proxyuser to your proxy user
- Change proxypwd to your proxy password
- Change proxy.server.com to the URL of your proxy server
- Change 8080 to the proxy port configured on your proxy server

## If you decide to reset proxy

$ git config --global --unset http.proxy

## To check the currently set proxy:

$ git config --global --get http.proxy
