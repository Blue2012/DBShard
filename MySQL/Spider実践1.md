# MariaDBのインストール

以下の順序で実践。

__1.レポジトリ追加__

```
vi /etc/yum.repos.d/mariadb.repo
```

```
# MariaDB 10.0 CentOS repository list - created 2014-04-02 07:21 UTC
# http://mariadb.org/mariadb/repositories/
[mariadb]
name = MariaDB
baseurl = http://yum.mariadb.org/10.1/centos7-amd64
gpgkey=https://yum.mariadb.org/RPM-GPG-KEY-MariaDB
gpgcheck=1
enabled=0
```

__2.インストール__

```
yum install --enablerepo=mariadb MariaDB-client MariaDB-devel MariaDB-server MariaDB-shared
```


