# Github 镜像备份
KANGLE_VERSION="3.5.8"
PHP_VERSION="5.2.17"
EASYPANEL_VERSION="2.6.18"
PUREFTP_VERSION="1.0.36"
PREFIX="/vhs/kangle"

## install-01.sh
yum -y install wget;wget https://github.com/potala2008/easypanel/raw/master/shell/install-01.sh -O install-01.sh;sh install-01.sh

## install-02.sh
yum -y install wget;wget https://github.com/potala2008/easypanel/raw/master/shell/install-02.sh -O install-02.sh;sh install-02.sh
