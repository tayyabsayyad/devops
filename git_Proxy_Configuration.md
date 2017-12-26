
# Git proxy server configuration 

git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080

    change proxyuser to your proxy user
    change proxypwd to your proxy password
    change proxy.server.com to the URL of your proxy server
    change 8080 to the proxy port configured on your proxy server

If you decide at any time to reset this proxy and work without proxy:

Command to use:

git config --global --unset http.proxy

Finally, to check the currently set proxy:

git config --global --get http.proxy

git config --global http.proxy http://tayyabali:Admin+1234@10.0.1.149:8060

