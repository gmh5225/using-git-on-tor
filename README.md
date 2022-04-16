# using-git-on-tor

# Guide
- Download https://github.com/shunf4/proxychains-windows
- Add environment variable PROXYCHAINS_CONF_FILE -> your proxychains bin\proxychains.conf
- Edit proxychains.conf and find [ProxyList] then change to socks5 127.0.0.1 9150
- proxychains_win32_x64.exe git clone http://rexw3wrz5pldtadf3hy4vqnuzokhco4l32kyntj36fcgpjuy3nvxidid.onion/gmh5225/Theodosius.git

# Easy Way
Enable:
```bash
git config --global http.proxy "socks5h://127.0.0.1:9150"
```
Disable:
```bash
git config --global --unset http.proxy
```

# Reference
- https://stackoverflow.com/questions/40857891/can-anyone-access-pluggable-transports-meek-git
