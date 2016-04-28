# sudo-openldap

Config sudo for ldap server

Copy sudo.ldif and sudo.schema to ldap server => path /etc/openldap/shcema

In terminal
$ ldapadd -Y EXTERNAL -H ldapi:/// -f sudo.ldif
$ service slapd restart
