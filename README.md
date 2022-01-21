# Uninstall old versions of Hortonworks/Cloudera software

## Setup test in newly installed CentOS machine

Install two repos like this:
> sudo yum install -y yum-utils

> sudo yum-config-manager \
>    --add-repo \
>    https://download.docker.com/linux/centos/docker-ce.repo

> sudo yum localinstall --nogpgcheck https://download1.rpmfusion.org/free/el/rpmfusion-free-release-7.noarch.rpm

## When testing, restore packages like this

> sudo yum install -y docker-ce docker-ce-cli containerd.io wireguard.noarch

After this run the playbook to uninstall these.

## How-to identify Hortonworks/Cloudera packages

> yum repolist | grep -i HDP

> yumdb search from_repo HDP-3.1-repo-301
