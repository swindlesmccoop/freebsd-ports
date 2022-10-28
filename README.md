# Usage
[Set up the ports tree](https://docs.freebsd.org/en/books/handbook/ports/#ports-using-installation-methods)
```
git clone https://git.cbps.xyz/swindlesmccoop/openbsd-ports/
doas cp -r openbsd-ports/* /usr/ports/mystuff/
cd /usr/ports/mystuff/[package]
su
make
```