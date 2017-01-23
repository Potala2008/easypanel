# 备用节点
PHP探针里面的服务器名根据节点去手工修改
完成后提交给域名管理员告诉他相关节点增加的服务器IP地址

### install-01.sh
wget https://potala2008.github.io/easypanel/shell/install-01.sh && sh install-01.sh

### install-02.sh
wget https://potala2008.github.io/easypanel/shell/install-02.sh && sh install-02.sh

### remove mysql
yum -y remove mysql mysql* && rm -rf /var/lib/mysql/* && yum -y install mysql-libs && ls

### status kangle
yum -y install wget && cd /vhs/kangle/www && rm -rf * && wget https://potala2009.github.io/bhs20091010/100MB.test && wget https://potala2009.github.io/bhs20091011/index.html && cd /vhs/kangle/nodewww/webftp/admin && rm -rf status.php && wget https://potala2009.github.io/bhs20091011/status.php && cd /root && rm -rf * && ls

### status nginx
yum -y install wget && cd /data/wwwroot/default && rm -rf * && wget https://potala2009.github.io/bhs20091010/100MB.test && wget https://potala2009.github.io/bhs20091011/index.html && cd /root && ls

### vhost.conf
cd /usr/local/nginx/conf && mkdir vhost && cd vhost && wget https://potala2009.github.io/bhs20091011/storage/vhost/PINSEYUN_store.conf && wget https://potala2009.github.io/bhs20091011/storage/vhost/PINSEYUN_down.conf && cd /root && ls

### status.conf
yum -y install epel-release && yum -y install python-pip && yum clean all && yum -y install gcc && yum -y install python-devel && pip install psutil && cd /root && mkdir storage && cd storage && mkdir status && cd status && wget https://potala2009.github.io/bhs20091011/storage/status/client.py && echo "nohup python /root/storage/status/client.py &> /dev/null &" >> /etc/rc.d/rc.local && cd /root && ls
