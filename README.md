# 备用节点
PHP探针里面的服务器名根据节点去手工修改
完成后提交给域名管理员告诉他相关节点增加的服务器IP地址

### install-01.sh
wget --no-check-certificate https://github.com/potala2008/easypanel/raw/master/shell/install-01.sh && sh install-01.sh

### install-02.sh
wget --no-check-certificate https://github.com/potala2008/easypanel/raw/master/shell/install-02.sh && sh install-02.sh

### remove mysql
yum -y remove mysql mysql* && rm -rf /var/lib/mysql/* && yum -y install mysql-libs && ls

### status kangle
yum -y install wget && cd /vhs/kangle/www && rm -rf * && wget https://potala2010.github.io/bhs20105010/100MB.test && wget https://potala2010.github.io/bhs20105020/index.html && cd /vhs/kangle/nodewww/webftp/admin && rm -rf status.php && wget https://potala2010.github.io/bhs20105020/status.php && cd /root && rm -rf * && ls

### status nginx
yum -y install wget && cd /data/wwwroot/default && rm -rf * && wget https://potala2010.github.io/bhs20105010/100MB.test && wget https://potala2010.github.io/bhs20105020/index.html && cd /root && ls