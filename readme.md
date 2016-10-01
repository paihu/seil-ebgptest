# BGP test use SEIL/x86


## Overview

SEIL is not support EBGP-multihop

This test is EBGP over ipsec


## before this use

1. install Virtualbox from (Virtualbox Website)[https://www.virtualbox.org/wiki/Downloads]
1. install Vagrant from (HasiCorp)[https://www.vagrantup.com/downloads.html]
1. install vagrant-plugin-seil
1. install SEIL Vagrant box from (SEIL/x86 Fuji download)[https://www.seil.jp/support/release/download_vm.html]
1. get seil starterkey (this page)[https://www.seil.jp/seilx86_download/download.php]
1. put starterkey.txt in this directory
1. install SEIL Linux debian8 box


## topology

[seil-1] --- [Debian8] --- [seil-2]


## case
## case1
default EBGP peering.
this case is not peering
## case2
use ipsec tunnel
this case is perring. but not accepted prefixes
## case3
use ipsec interface
this case is peering and accepted prefixes.
but next-hop is over ipsec interface

