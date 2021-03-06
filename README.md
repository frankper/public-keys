Table of Contents
=================

   * [public-keys](#public-keys)
      * [To import all my ssh and gpg keys](#to-import-all-my-ssh-and-gpg-keys)
      * [To import only my ssh keys](#to-import-only-my-ssh-keys)
      * [To import only my gpg keys](#to-import-only-my-gpg-keys)
         * [From Ubuntu GPG keyserver](#from-ubuntu-gpg-keyserver)
         * [From my gitlab repo](#from-my-gitlab-repo)
   * [repo tree](#repo-tree)

Created by [gh-md-toc](https://github.com/ekalinin/github-markdown-toc)
# public-keys
My public ssh and gpg keys 

Make sure **gpg** and **curl** is installed in your system before attempting any of the following 

## To import all my ssh and gpg keys
Fetch and run the script 
```shell
bash <(curl -fsSL https://gitlab.com/frankper/public-keys/-/raw/master/install_frank.sh) -a
```
## To import only my ssh keys
```shell
bash <(curl -fsSL https://gitlab.com/frankper/public-keys/-/raw/master/install_frank.sh) -s 
```
## To import only my gpg keys
### From Ubuntu GPG keyserver
```shell
bash <(curl -fsSL https://gitlab.com/frankper/public-keys/-/raw/master/install_frank.sh) -u
```
### From my gitlab repo
```shell
bash <(curl -fsSL https://gitlab.com/frankper/public-keys/-/raw/master/install_frank.sh) -g
```
# repo tree
```shell
0 directories, 9 files
.
├── authorized_keys
├── frank.perrakis.gpg001.asc
├── frank.perrakis.gpg002.asc
├── frank.perrakis.gpg003.v2-v3.asc
├── frank.perrakis.yubikey.asc
├── gpg-keys-urls
├── install_frank.sh
├── README.md
└── rsync_keys.sh
```