# public-keys
My public ssh and gpg keys 

Make sure **gpg** and **curl** is installed in your system before attempting any of the following 

## To import all my ssh keys type 
```shell
curl -sSL https://raw.githubusercontent.com/frankper/public-keys/master/authorized_keys >> ~/.ssh/authorized_keys
```
## To import all my gpg keys 

### From gpg keyservers 

```shell
# yubikey
curl -sSL https://keyserver.ubuntu.com/pks/lookup\?op\=get\&search\=0x5faddad63d31b26a | gpg --import -
# gpg card 001 
curl -sSL https://keybase.io/koulis1984/pgp_keys.asc?fingerprint=5de1fc59303a7db59b26bd57a59e931a849979fc | gpg --import -
```
### From github repo
```shell
# yubikey 
curl -sSL https://raw.githubusercontent.com/frankper/public-keys/master/frank.perrakis.yubikey.asc | gpg --import -
# gpg card 001 
curl -sSL https://raw.githubusercontent.com/frankper/public-keys/master/frank.perrakis.gpg001.asc | gpg --import -
```

