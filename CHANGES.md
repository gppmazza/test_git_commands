Changes in the committed version of the role:

20180523:
- initial hp:
  ```
  root@selby-vm1:~# grep kerberos /etc/krb5.conf
                  kdc = kerberos.doc.ic.ac.uk
  ```
  all the following commands work fine:
  ```
  ssh gmazza@selby-vm1
  gmazza@selby-vm1:~$ ksu
  root@selby-vm1:/home/gmazza#
  gmazza@selby-vm1:~$ su
  # in this case you will get the CSG msg "sudont":
  gmazza@selby-vm1:~$ sudo /bin/bash
  ```
