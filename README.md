# Uninstall old versions of Hortonworks/Cloudera software

## When testing, restore packages like this

> dnf install -y adobe-mappings-cmap-20171205-4.fc29.noarch

## How-to identify Hortonworks/Cloudera packages

> yum repolist | grep -i HDP

> yumdb search from_repo HDP-3.1-repo-301
