# Gluu server

Edit `config.yaml` and finish installatioin of Gluu Server

```sh
> vagrant ssh
$ sudo /sbin/gluu-serverd-3.1.2 login
# cd /install/community-edition-setup/
# ./setup.py -asr -e -n -f ./setup.properties
```

## Base box

see base branch.

## TODO

gluu setup.py `-cas` options doesn't work with default properties.

```sh
# ./setup.py -cas -e -n -f ./setup.properties
```

If you want install install CAS, Shibboleth SAML IDP and Asimba SAML Proxy, you should setup manually.

```sh
> vagrant ssh
$ sudo /sbin/gluu-serverd-3.1.2 login
# cd /install/community-edition-setup/
# ./setup.py
```

```sh
Install oxAuth OAuth2 Authorization Server? [Yes] :
Install oxTrust Admin UI? [Yes] :
Install LDAP Server? [Yes] :
Install (1) Gluu OpenDJ (2) OpenLDAP Gluu Edition [1|2] [1] :
Install Apache HTTPD Server [Yes] :
Install Shibboleth SAML IDP? [No] : y
Install Asimba SAML Proxy? [No] : y
Install oxAuth RP? [No] : y
Install Passport? [No] : y
Install JCE 1.8? [Yes] : y
```