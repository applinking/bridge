# bridge

A tiny static page that opens a custom URL scheme from a link you can tap anywhere.

```
https://applinking.github.io/bridge/#<scheme>://<rest>
```

Everything after `#` is handled in the browser and is never sent to the server.
The page collects nothing and loads no third-party scripts.

Web and dangerous schemes (`http`, `https`, `ftp`, `ws`, `wss`, `javascript`, `data`, `file`, `blob`, `about`, `vbscript`, `itms-services`) are refused; the target may only contain letters, digits and `_-./?=&%:~+`, up to 512 characters.
