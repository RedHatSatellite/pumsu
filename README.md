This script allows you to build and upload puppet modules into Satellite 6

Example output:
```sh
[root@sat ~]# ./pumsu --modules module_list.txt --source puppet-modules/ --repoid 9
[*] building module: abrt_ccpp
[*] building module: abrtd
[*] building module: abrt_oops
[*] building module: accts_lock
[*] building module: accts_nologin
[*] building module: atd
[*] building module: auditd
[*] building module: authorized_keys
[*] building module: avahi
[*] building module: chrony
[*] building module: cpumgmt
[*] building module: crond
[*] building module: dbus
[*] building module: device_drivers
[*] building module: dnsmasq
[*] building module: ebtables
[*] building module: extra_facts
[*] building module: filesystems
[*] building module: firewalld
[*] building module: gofer
[*] building module: grub2
[*] building module: haldaemon
[*] building module: hosts
[*] building module: init
[*] building module: ip6tables
[*] building module: iptables
[*] building module: irqbalance
[*] building module: issue
[*] building module: kdump
[*] building module: limits
[*] building module: login_defs
[*] building module: lvm2_lvmetad
[*] building module: lvm2_monitor
[*] building module: mdmonitor
[*] building module: mlocate
[*] building module: motd
[*] building module: netfs
[*] building module: ntp
[*] building module: ntpdate
[*] building module: oddjob
[*] building module: pam_login
[*] building module: password_quality
[*] building module: postfix
[*] building module: profiles
[*] building module: protocols
[*] building module: psacct
[*] building module: puppet
[*] building module: quota_nld
[*] building module: rdisc
[*] building module: restorecond
[*] building module: rhfuncs
[*] building module: rhnsd
[*] building module: rhsmcertd
[*] building module: rsyslog
[*] building module: saslauthd
[*] building module: scheduling
[*] building module: securetty
[*] building module: selinux
[*] building module: shadow
[*] building module: smartd
[*] building module: snmp
[*] building module: sshd
[*] building module: su
[*] building module: sudoers
[*] building module: sysctl
[*] building module: sysstat
[*] building module: tcpwrappers
[*] building module: tuned
[*] building module: udev_rules
[*] building module: useradd_defs
[*] building module: users
[*] building module: xinetd
[*] uploading modules
[*] cleaning up temp dir
[root@sat ~]# hammer repository info --id 9
...
Content Counts:     
    Puppet Modules: 74

```

