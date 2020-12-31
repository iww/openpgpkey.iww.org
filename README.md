On system with @iww.org keys, in directory **.well-known** run:

```
gpg --list-options show-only-fpr-mbox -k "@iww.org" | $(gpgconf --list-dirs libexecdir)/gpg-wks-client -v --install-key
```

*Requires **GPG >= 2.2.12** with **gpg-wks-client** (on macOS, must compile from [source](https://gnupg.org/download/index.html))* 

References:
- https://wiki.gnupg.org/WKDHosting
- https://github.com/mihalyr/openpgpkey
