# check_asterisk_pjsip
Icinga/nagios check for asterisk/freebox pjsip registrations/endpoints

## instructions

make sure your `nagios` user can run `asterisk -x` commands, i.e.
```
groupmems -a nagios -g asterisk
```

## test

```
[root@freepbx nrpe.d]# sudo -u nagios /usr/local/bin/check_asterisk_pjsip -r SRV3  -e PS1 -e PS2 -e SRV3
OK: Registration status for SRV3 is Registered
OK: Endpoint status for PS1 is Avail
OK: Endpoint status for PS2 is Avail
OK: Endpoint status for SRV3 is Avail
```

