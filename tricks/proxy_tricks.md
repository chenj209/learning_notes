# Proxy tricks

### To test if proxy works in terminal
1. curl cip.cc
2. curl ip.cn
3. curl ip.sb

### To test with proxy port
1. curl cip.cc/curl -x "proxyserver" cip.cc
2. curl http://httpbin.org/ip/curl -x "proxyserver" http://httpbin.org/ip
3. curl --socks5 "socket5server" cip.cc
